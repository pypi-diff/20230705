# Comparing `tmp/deepsecrets-1.1.0.tar.gz` & `tmp/deepsecrets-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsecrets-1.1.0.tar", max compression
+gzip compressed data, was "deepsecrets-1.1.1.tar", max compression
```

## Comparing `deepsecrets-1.1.0.tar` & `deepsecrets-1.1.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.1.0/LICENSE
--rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.1.0/README.md
--rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.1.0/deepsecrets/.DS_Store
--rw-r--r--   0        0        0      674 2023-07-04 12:10:29.237681 deepsecrets-1.1.0/deepsecrets/__init__.py
--rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.1.0/deepsecrets/__main__.py
--rw-r--r--   0        0        0     7633 2023-07-04 11:57:11.643286 deepsecrets-1.1.0/deepsecrets/cli.py
--rw-r--r--   0        0        0     2256 2023-07-03 10:00:00.045463 deepsecrets-1.1.0/deepsecrets/config.py
--rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/.DS_Store
--rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.1.0/deepsecrets/core/engines/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     6192 2023-06-27 14:07:40.467355 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.1.0/deepsecrets/core/engines/hashed_secret.py
--rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.1.0/deepsecrets/core/engines/iengine.py
--rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.1.0/deepsecrets/core/engines/regex.py
--rw-r--r--   0        0        0     4341 2023-06-27 14:07:39.916706 deepsecrets-1.1.0/deepsecrets/core/engines/semantic.py
--rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
--rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
--rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/content_analyzer.py
--rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.1.0/deepsecrets/core/helpers/entropy.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/model/.DS_Store
--rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.1.0/deepsecrets/core/model/__init__.py
--rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7355 2023-06-28 16:55:39.241507 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
--rw-r--r--   0        0        0      797 2023-06-28 18:04:12.582631 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     3926 2023-07-04 13:26:48.391130 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     3886 2023-06-28 16:55:38.707373 deepsecrets-1.1.0/deepsecrets/core/model/file.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.1.0/deepsecrets/core/model/finding.py
--rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/__init__.py
--rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
--rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
--rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/exlcuded_path.py
--rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.1.0/deepsecrets/core/model/rules/false_finding.py
--rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.1.0/deepsecrets/core/model/rules/hashed_secret.py
--rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.1.0/deepsecrets/core/model/rules/hashing.py
--rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.1.0/deepsecrets/core/model/rules/regex.py
--rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.1.0/deepsecrets/core/model/rules/rule.py
--rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/semantic.py
--rw-r--r--   0        0        0      281 2023-06-28 18:04:11.970796 deepsecrets-1.1.0/deepsecrets/core/model/semantic.py
--rw-r--r--   0        0        0     2007 2023-07-04 13:26:47.808614 deepsecrets-1.1.0/deepsecrets/core/model/token.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/modes/.DS_Store
--rw-r--r--   0        0        0     8594 2023-07-04 09:53:49.065871 deepsecrets-1.1.0/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
--rw-r--r--   0        0        0     5166 2023-07-04 09:53:48.500643 deepsecrets-1.1.0/deepsecrets/core/modes/iscan_mode.py
--rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
--rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
--rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
--rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
--rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
--rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
--rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
--rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
--rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
--rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
--rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
--rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/excluded_paths.py
--rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.1.0/deepsecrets/core/rulesets/false_findings.py
--rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.1.0/deepsecrets/core/rulesets/hashed_secrets.py
--rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/ibuilder.py
--rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/regex.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/.DS_Store
--rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__init__.py
--rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
--rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
--rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
--rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
--rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
--rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
--rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
--rw-r--r--   0        0        0    10945 2023-07-04 12:01:13.022231 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
--rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
--rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
--rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
--rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
--rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
--rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/full_content.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-06-28 17:29:54.564568 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
--rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1371 2023-06-28 18:14:23.816502 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
--rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
--rw-r--r--   0        0        0      556 2023-06-28 18:14:23.216059 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/language.py
--rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
--rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7398 2023-06-28 18:18:53.090440 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
--rw-r--r--   0        0        0     7425 2023-07-04 13:39:06.736554 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     3845 2023-06-28 18:18:52.403328 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
--rw-r--r--   0        0        0     6529 2023-07-04 13:39:05.813218 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
--rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/spot_improvements.py
--rw-r--r--   0        0        0     1801 2023-06-28 17:29:53.978332 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/type_stream.py
--rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/itokenizer.py
--rw-r--r--   0        0        0     6862 2023-07-04 12:01:12.367278 deepsecrets-1.1.0/deepsecrets/core/tokenizers/lexer.py
--rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_line.py
--rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_word.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/utils/.DS_Store
--rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3487 2023-07-03 09:28:55.083680 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc
--rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     5474 2023-07-04 09:56:49.777143 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
--rw-r--r--   0        0        0     2681 2023-06-30 18:34:33.195619 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
--rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5265 2023-07-03 12:07:13.918625 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc
--rw-r--r--   0        0        0     1759 2023-07-03 09:28:54.438041 deepsecrets-1.1.0/deepsecrets/core/utils/cpu.py
--rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.1.0/deepsecrets/core/utils/exceptions.py
--rw-r--r--   0        0        0     3022 2023-07-04 09:56:48.933550 deepsecrets-1.1.0/deepsecrets/core/utils/file_analyzer.py
--rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.1.0/deepsecrets/core/utils/fs.py
--rw-r--r--   0        0        0     1538 2023-06-30 18:34:31.705561 deepsecrets-1.1.0/deepsecrets/core/utils/guess_filetype.py
--rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.1.0/deepsecrets/core/utils/hashing.py
--rw-r--r--   0        0        0     2810 2023-07-03 12:07:13.137522 deepsecrets-1.1.0/deepsecrets/core/utils/lexer_finder.py
--rw-r--r--   0        0        0     2669 2023-07-04 14:27:00.175183 deepsecrets-1.1.0/deepsecrets/rules/excluded_paths.json
--rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.1.0/deepsecrets/rules/regexes.json
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/scan_modes/.DS_Store
--rw-r--r--   0        0        0     5823 2023-07-04 11:57:19.417209 deepsecrets-1.1.0/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     3333 2023-07-04 11:57:18.653455 deepsecrets-1.1.0/deepsecrets/scan_modes/cli.py
--rw-r--r--   0        0        0     1709 2023-07-03 11:58:13.505921 deepsecrets-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6274 1970-01-01 00:00:00.000000 deepsecrets-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.1.1/README.md
+-rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.1.1/deepsecrets/.DS_Store
+-rw-r--r--   0        0        0      674 2023-07-04 12:10:29.237681 deepsecrets-1.1.1/deepsecrets/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.1.1/deepsecrets/__main__.py
+-rw-r--r--   0        0        0     7633 2023-07-04 11:57:11.643286 deepsecrets-1.1.1/deepsecrets/cli.py
+-rw-r--r--   0        0        0     2256 2023-07-03 10:00:00.045463 deepsecrets-1.1.1/deepsecrets/config.py
+-rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/.DS_Store
+-rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.1.1/deepsecrets/core/engines/__init__.py
+-rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     6192 2023-06-27 14:07:40.467355 deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.1.1/deepsecrets/core/engines/hashed_secret.py
+-rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.1.1/deepsecrets/core/engines/iengine.py
+-rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.1.1/deepsecrets/core/engines/regex.py
+-rw-r--r--   0        0        0     4341 2023-06-27 14:07:39.916706 deepsecrets-1.1.1/deepsecrets/core/engines/semantic.py
+-rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
+-rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
+-rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.1.1/deepsecrets/core/helpers/content_analyzer.py
+-rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.1.1/deepsecrets/core/helpers/entropy.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/model/.DS_Store
+-rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.1.1/deepsecrets/core/model/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7355 2023-06-28 16:55:39.241507 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
+-rw-r--r--   0        0        0      797 2023-06-28 18:04:12.582631 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     3926 2023-07-04 13:26:48.391130 deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     3886 2023-06-28 16:55:38.707373 deepsecrets-1.1.1/deepsecrets/core/model/file.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.1.1/deepsecrets/core/model/finding.py
+-rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/__init__.py
+-rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
+-rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/exlcuded_path.py
+-rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.1.1/deepsecrets/core/model/rules/false_finding.py
+-rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.1.1/deepsecrets/core/model/rules/hashed_secret.py
+-rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.1.1/deepsecrets/core/model/rules/hashing.py
+-rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.1.1/deepsecrets/core/model/rules/regex.py
+-rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.1.1/deepsecrets/core/model/rules/rule.py
+-rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.1.1/deepsecrets/core/model/rules/semantic.py
+-rw-r--r--   0        0        0      281 2023-06-28 18:04:11.970796 deepsecrets-1.1.1/deepsecrets/core/model/semantic.py
+-rw-r--r--   0        0        0     2007 2023-07-04 13:26:47.808614 deepsecrets-1.1.1/deepsecrets/core/model/token.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/modes/.DS_Store
+-rw-r--r--   0        0        0     8594 2023-07-04 09:53:49.065871 deepsecrets-1.1.1/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
+-rw-r--r--   0        0        0     5166 2023-07-04 09:53:48.500643 deepsecrets-1.1.1/deepsecrets/core/modes/iscan_mode.py
+-rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
+-rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
+-rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
+-rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
+-rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
+-rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
+-rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
+-rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
+-rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
+-rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/excluded_paths.py
+-rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.1.1/deepsecrets/core/rulesets/false_findings.py
+-rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.1.1/deepsecrets/core/rulesets/hashed_secrets.py
+-rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/ibuilder.py
+-rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.1.1/deepsecrets/core/rulesets/regex.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/.DS_Store
+-rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
+-rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
+-rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
+-rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    10945 2023-07-04 12:01:13.022231 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
+-rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
+-rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
+-rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
+-rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/full_content.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-06-28 17:29:54.564568 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
+-rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1371 2023-06-28 18:14:23.816502 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
+-rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
+-rw-r--r--   0        0        0      556 2023-06-28 18:14:23.216059 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/language.py
+-rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7398 2023-06-28 18:18:53.090440 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
+-rw-r--r--   0        0        0     7425 2023-07-04 13:39:06.736554 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     3845 2023-06-28 18:18:52.403328 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
+-rw-r--r--   0        0        0     6529 2023-07-04 13:39:05.813218 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
+-rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/spot_improvements.py
+-rw-r--r--   0        0        0     1801 2023-06-28 17:29:53.978332 deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/type_stream.py
+-rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.1.1/deepsecrets/core/tokenizers/itokenizer.py
+-rw-r--r--   0        0        0     6862 2023-07-04 12:01:12.367278 deepsecrets-1.1.1/deepsecrets/core/tokenizers/lexer.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_line.py
+-rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_word.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/core/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3491 2023-07-05 06:48:16.796963 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc
+-rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     5474 2023-07-04 09:56:49.777143 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
+-rw-r--r--   0        0        0     2681 2023-06-30 18:34:33.195619 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
+-rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5265 2023-07-03 12:07:13.918625 deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc
+-rw-r--r--   0        0        0     1763 2023-07-05 06:48:16.188353 deepsecrets-1.1.1/deepsecrets/core/utils/cpu.py
+-rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.1.1/deepsecrets/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3022 2023-07-04 09:56:48.933550 deepsecrets-1.1.1/deepsecrets/core/utils/file_analyzer.py
+-rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.1.1/deepsecrets/core/utils/fs.py
+-rw-r--r--   0        0        0     1538 2023-06-30 18:34:31.705561 deepsecrets-1.1.1/deepsecrets/core/utils/guess_filetype.py
+-rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.1.1/deepsecrets/core/utils/hashing.py
+-rw-r--r--   0        0        0     2810 2023-07-03 12:07:13.137522 deepsecrets-1.1.1/deepsecrets/core/utils/lexer_finder.py
+-rw-r--r--   0        0        0     2669 2023-07-04 14:27:00.175183 deepsecrets-1.1.1/deepsecrets/rules/excluded_paths.json
+-rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.1.1/deepsecrets/rules/regexes.json
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.1/deepsecrets/scan_modes/.DS_Store
+-rw-r--r--   0        0        0     5823 2023-07-04 11:57:19.417209 deepsecrets-1.1.1/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3333 2023-07-04 11:57:18.653455 deepsecrets-1.1.1/deepsecrets/scan_modes/cli.py
+-rw-r--r--   0        0        0     1709 2023-07-05 06:48:55.892463 deepsecrets-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6274 1970-01-01 00:00:00.000000 deepsecrets-1.1.1/PKG-INFO
```

### Comparing `deepsecrets-1.1.0/LICENSE` & `deepsecrets-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/README.md` & `deepsecrets-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/__init__.py` & `deepsecrets-1.1.1/deepsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/cli.py` & `deepsecrets-1.1.1/deepsecrets/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/config.py` & `deepsecrets-1.1.1/deepsecrets/config.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/hashed_secret.py` & `deepsecrets-1.1.1/deepsecrets/core/engines/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/iengine.py` & `deepsecrets-1.1.1/deepsecrets/core/engines/iengine.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/regex.py` & `deepsecrets-1.1.1/deepsecrets/core/engines/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/engines/semantic.py` & `deepsecrets-1.1.1/deepsecrets/core/engines/semantic.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/helpers/content_analyzer.py` & `deepsecrets-1.1.1/deepsecrets/core/helpers/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/helpers/entropy.py` & `deepsecrets-1.1.1/deepsecrets/core/helpers/entropy.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/core/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/file.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/token.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/__pycache__/token.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/file.py` & `deepsecrets-1.1.1/deepsecrets/core/model/file.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/finding.py` & `deepsecrets-1.1.1/deepsecrets/core/model/finding.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/rules/hashed_secret.py` & `deepsecrets-1.1.1/deepsecrets/core/model/rules/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/rules/regex.py` & `deepsecrets-1.1.1/deepsecrets/core/model/rules/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/rules/rule.py` & `deepsecrets-1.1.1/deepsecrets/core/model/rules/rule.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/model/token.py` & `deepsecrets-1.1.1/deepsecrets/core/model/token.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/modes/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/core/modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/modes/iscan_mode.py` & `deepsecrets-1.1.1/deepsecrets/core/modes/iscan_mode.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/hashed_secrets.py` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/hashed_secrets.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/rulesets/ibuilder.py` & `deepsecrets-1.1.1/deepsecrets/core/rulesets/ibuilder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/language.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/language.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/spot_improvements.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/spot_improvements.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/type_stream.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/helpers/type_stream.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/itokenizer.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/itokenizer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/lexer.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/lexer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_line.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_line.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_word.py` & `deepsecrets-1.1.1/deepsecrets/core/tokenizers/per_word.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/core/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd694a264 (Mon Jul  3 09:28:54 2023 UTC)
-files sz: 1759
+moddate:  0x3012a564 (Wed Jul  5 06:48:16 2023 UTC)
+files sz: 1763
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a03010064035a
@@ -174,131 +174,131 @@
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x970064017d0164027d0274010000000000000000000074020000000000
-                  0000000000a6010000ab010000000000000000722c09007c00a002000000
+                  0000000000a6010000ab010000000000000000722d09007c00a002000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
-                  005c0200007d017d027c017c026602530023007406000000000000000000
-                  0024007203010059006e0477007803590077017401000000000000000000
-                  00740800000000000000000000a6010000ab010000000000000000724074
-                  0100000000000000000000740a00000000000000000000a6010000ab0100
-                  00000000000000722c09007c00a006000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000005c0200007d017d027c017c
-                  0266025300230074060000000000000000000024007203010059006e0477
-                  007803590077017c017c027a0200005300
+                  005c0200007d017d027c017c027a02000053002300740600000000000000
+                  00000024007203010059006e047700780359007701740100000000000000
+                  000000740800000000000000000000a6010000ab01000000000000000072
+                  41740100000000000000000000740a00000000000000000000a6010000ab
+                  010000000000000000722d09007c00a00600000000000000000000000000
+                  00000000000000a6000000ab0000000000000000005c0200007d017d027c
+                  017c027a0200005300230074060000000000000000000024007203010059
+                  006e0477007803590077017c017c027a0200005300
                 22           0 RESUME                   0
                
                 23           2 LOAD_CONST               1 (1)
                              4 STORE_FAST               1 (quota)
                
                 24           6 LOAD_CONST               2 (-1)
                              8 STORE_FAST               2 (period)
                
                 27          10 LOAD_GLOBAL              1 (NULL + path_exists)
                             22 LOAD_GLOBAL              2 (CGROUP_2_MAX)
                             34 PRECALL                  1
                             38 CALL                     1
-                            48 POP_JUMP_FORWARD_IF_FALSE    44 (to 138)
+                            48 POP_JUMP_FORWARD_IF_FALSE    45 (to 140)
                
                 28          50 NOP
                
                 29          52 LOAD_FAST                0 (self)
                             54 LOAD_METHOD              2 (_CpuHelper__cgroup2)
                             76 PRECALL                  0
                             80 CALL                     0
                             90 UNPACK_SEQUENCE          2
                             94 STORE_FAST               1 (quota)
                             96 STORE_FAST               2 (period)
                
                 30          98 LOAD_FAST                1 (quota)
                            100 LOAD_FAST                2 (period)
-                           102 BUILD_TUPLE              2
-                           104 RETURN_VALUE
-                       >>  106 PUSH_EXC_INFO
-               
-                31         108 LOAD_GLOBAL              6 (Exception)
-                           120 CHECK_EXC_MATCH
-                           122 POP_JUMP_FORWARD_IF_FALSE     3 (to 130)
-                           124 POP_TOP
-               
-                32         126 POP_EXCEPT
-                           128 JUMP_FORWARD             4 (to 138)
-               
-                31     >>  130 RERAISE                  0
-                       >>  132 COPY                     3
-                           134 POP_EXCEPT
-                           136 RERAISE                  1
-               
-                35     >>  138 LOAD_GLOBAL              1 (NULL + path_exists)
-                           150 LOAD_GLOBAL              8 (QUOTA_FILE)
-                           162 PRECALL                  1
-                           166 CALL                     1
-                           176 POP_JUMP_FORWARD_IF_FALSE    64 (to 306)
-                           178 LOAD_GLOBAL              1 (NULL + path_exists)
-                           190 LOAD_GLOBAL             10 (PERIOD_FILE)
-                           202 PRECALL                  1
-                           206 CALL                     1
-                           216 POP_JUMP_FORWARD_IF_FALSE    44 (to 306)
-               
-                36         218 NOP
-               
-                37         220 LOAD_FAST                0 (self)
-                           222 LOAD_METHOD              6 (_CpuHelper__cgroup1)
-                           244 PRECALL                  0
-                           248 CALL                     0
-                           258 UNPACK_SEQUENCE          2
-                           262 STORE_FAST               1 (quota)
-                           264 STORE_FAST               2 (period)
-               
-                38         266 LOAD_FAST                1 (quota)
-                           268 LOAD_FAST                2 (period)
-                           270 BUILD_TUPLE              2
-                           272 RETURN_VALUE
-                       >>  274 PUSH_EXC_INFO
-               
-                39         276 LOAD_GLOBAL              6 (Exception)
-                           288 CHECK_EXC_MATCH
-                           290 POP_JUMP_FORWARD_IF_FALSE     3 (to 298)
-                           292 POP_TOP
-               
-                40         294 POP_EXCEPT
-                           296 JUMP_FORWARD             4 (to 306)
-               
-                39     >>  298 RERAISE                  0
-                       >>  300 COPY                     3
-                           302 POP_EXCEPT
-                           304 RERAISE                  1
-               
-                42     >>  306 LOAD_FAST                1 (quota)
-                           308 LOAD_FAST                2 (period)
-                           310 BINARY_OP                2 (//)
-                           314 RETURN_VALUE
+                           102 BINARY_OP                2 (//)
+                           106 RETURN_VALUE
+                       >>  108 PUSH_EXC_INFO
+               
+                31         110 LOAD_GLOBAL              6 (Exception)
+                           122 CHECK_EXC_MATCH
+                           124 POP_JUMP_FORWARD_IF_FALSE     3 (to 132)
+                           126 POP_TOP
+               
+                32         128 POP_EXCEPT
+                           130 JUMP_FORWARD             4 (to 140)
+               
+                31     >>  132 RERAISE                  0
+                       >>  134 COPY                     3
+                           136 POP_EXCEPT
+                           138 RERAISE                  1
+               
+                35     >>  140 LOAD_GLOBAL              1 (NULL + path_exists)
+                           152 LOAD_GLOBAL              8 (QUOTA_FILE)
+                           164 PRECALL                  1
+                           168 CALL                     1
+                           178 POP_JUMP_FORWARD_IF_FALSE    65 (to 310)
+                           180 LOAD_GLOBAL              1 (NULL + path_exists)
+                           192 LOAD_GLOBAL             10 (PERIOD_FILE)
+                           204 PRECALL                  1
+                           208 CALL                     1
+                           218 POP_JUMP_FORWARD_IF_FALSE    45 (to 310)
+               
+                36         220 NOP
+               
+                37         222 LOAD_FAST                0 (self)
+                           224 LOAD_METHOD              6 (_CpuHelper__cgroup1)
+                           246 PRECALL                  0
+                           250 CALL                     0
+                           260 UNPACK_SEQUENCE          2
+                           264 STORE_FAST               1 (quota)
+                           266 STORE_FAST               2 (period)
+               
+                38         268 LOAD_FAST                1 (quota)
+                           270 LOAD_FAST                2 (period)
+                           272 BINARY_OP                2 (//)
+                           276 RETURN_VALUE
+                       >>  278 PUSH_EXC_INFO
+               
+                39         280 LOAD_GLOBAL              6 (Exception)
+                           292 CHECK_EXC_MATCH
+                           294 POP_JUMP_FORWARD_IF_FALSE     3 (to 302)
+                           296 POP_TOP
+               
+                40         298 POP_EXCEPT
+                           300 JUMP_FORWARD             4 (to 310)
+               
+                39     >>  302 RERAISE                  0
+                       >>  304 COPY                     3
+                           306 POP_EXCEPT
+                           308 RERAISE                  1
+               
+                42     >>  310 LOAD_FAST                1 (quota)
+                           312 LOAD_FAST                2 (period)
+                           314 BINARY_OP                2 (//)
+                           318 RETURN_VALUE
                ExceptionTable:
-                 52 to 102 -> 106 [0]
-                 106 to 124 -> 132 [1] lasti
-                 130 to 130 -> 132 [1] lasti
-                 220 to 270 -> 274 [0]
-                 274 to 292 -> 300 [1] lasti
-                 298 to 298 -> 300 [1] lasti
+                 52 to 104 -> 108 [0]
+                 108 to 126 -> 134 [1] lasti
+                 132 to 132 -> 134 [1] lasti
+                 222 to 274 -> 278 [0]
+                 278 to 296 -> 304 [1] lasti
+                 302 to 302 -> 304 [1] lasti
                consts
                   None
                   1
                   -1
                names      ('path_exists', 'CGROUP_2_MAX', '_CpuHelper__cgroup2', 'Exception', 'QUOTA_FILE', 'PERIOD_FILE', '_CpuHelper__cgroup1')
                varnames   ('self', 'quota', 'period')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/utils/cpu.py'
                name       '_by_cgroup'
                firstlineno 22
                lnotab
-                  0x020104010403280102012e010a01120104ff0804500102012e010a0112
+                  0x020104010403280102012e010c01120104ff0804500102012e010c0112
                   0104ff0803
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
```

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/cpu.py` & `deepsecrets-1.1.1/deepsecrets/core/utils/cpu.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,23 +23,23 @@
         quota = 1
         period = -1
 
 	    # cgroup 2: https://www.kernel.org/doc/html/latest/admin-guide/cgroup-v2.html
         if path_exists(CGROUP_2_MAX):
             try:
                 quota, period = self.__cgroup2()
-                return quota, period
+                return quota // period
             except Exception:
                 pass
 
         # cgroup 1: https://www.kernel.org/doc/html/latest/admin-guide/cgroup-v1/index.html
         if path_exists(QUOTA_FILE) and path_exists(PERIOD_FILE):
             try:
                 quota, period = self.__cgroup1()
-                return quota, period
+                return quota // period
             except Exception:
                 pass
 
         return quota // period
     
     def __cgroup1(self):
         quota = 1
```

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/file_analyzer.py` & `deepsecrets-1.1.1/deepsecrets/core/utils/file_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/fs.py` & `deepsecrets-1.1.1/deepsecrets/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/guess_filetype.py` & `deepsecrets-1.1.1/deepsecrets/core/utils/guess_filetype.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/hashing.py` & `deepsecrets-1.1.1/deepsecrets/core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/core/utils/lexer_finder.py` & `deepsecrets-1.1.1/deepsecrets/core/utils/lexer_finder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/rules/excluded_paths.json` & `deepsecrets-1.1.1/deepsecrets/rules/excluded_paths.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/rules/regexes.json` & `deepsecrets-1.1.1/deepsecrets/rules/regexes.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/scan_modes/.DS_Store` & `deepsecrets-1.1.1/deepsecrets/scan_modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc` & `deepsecrets-1.1.1/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/deepsecrets/scan_modes/cli.py` & `deepsecrets-1.1.1/deepsecrets/scan_modes/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.1.0/pyproject.toml` & `deepsecrets-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsecrets"
-version = "1.1.0"
+version = "1.1.1"
 description = "A better tool for secrets search"
 license = "MIT"
 authors = [
   "Nikolai Khechumov <khechumov@gmail.com>",
 ]
 keywords = ["security", "secrets", "credentials", "scanning", "appsec"]
 packages = [{include = "deepsecrets"}]
```

### Comparing `deepsecrets-1.1.0/PKG-INFO` & `deepsecrets-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsecrets
-Version: 1.1.0
+Version: 1.1.1
 Summary: A better tool for secrets search
 License: MIT
 Keywords: security,secrets,credentials,scanning,appsec
 Author: Nikolai Khechumov
 Author-email: khechumov@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
```

