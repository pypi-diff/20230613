# Comparing `tmp/deepsecrets-1.0.3.tar.gz` & `tmp/deepsecrets-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsecrets-1.0.3.tar", max compression
+gzip compressed data, was "deepsecrets-1.0.4.tar", max compression
```

## Comparing `deepsecrets-1.0.3.tar` & `deepsecrets-1.0.4.tar`

### file list

```diff
@@ -1,145 +1,144 @@
--rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.3/LICENSE
--rw-r--r--   0        0        0     3889 2023-04-22 04:46:27.734564 deepsecrets-1.0.3/README.md
--rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.3/deepsecrets/.DS_Store
--rw-r--r--   0        0        0      674 2023-04-27 13:31:17.046975 deepsecrets-1.0.3/deepsecrets/__init__.py
--rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.0.3/deepsecrets/__main__.py
--rw-r--r--   0        0        0     6429 2023-04-17 13:31:34.040560 deepsecrets-1.0.3/deepsecrets/cli.py
--rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.3/deepsecrets/config.py
--rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/core/.DS_Store
--rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.3/deepsecrets/core/engines/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-04-17 13:35:10.334351 deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     6184 2023-04-14 12:59:29.927306 deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.3/deepsecrets/core/engines/hashed_secret.py
--rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.3/deepsecrets/core/engines/iengine.py
--rw-r--r--   0        0        0     1196 2023-04-17 13:35:09.681785 deepsecrets-1.0.3/deepsecrets/core/engines/regex.py
--rw-r--r--   0        0        0     4333 2023-04-14 12:59:29.251562 deepsecrets-1.0.3/deepsecrets/core/engines/semantic.py
--rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
--rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
--rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.3/deepsecrets/core/helpers/content_analyzer.py
--rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.3/deepsecrets/core/helpers/entropy.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/core/model/.DS_Store
--rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.3/deepsecrets/core/model/__init__.py
--rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6910 2023-04-14 13:22:42.127475 deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
--rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     3719 2023-04-14 13:22:41.393440 deepsecrets-1.0.3/deepsecrets/core/model/file.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.3/deepsecrets/core/model/finding.py
--rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.3/deepsecrets/core/model/rules/__init__.py
--rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
--rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
--rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.3/deepsecrets/core/model/rules/exlcuded_path.py
--rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.3/deepsecrets/core/model/rules/false_finding.py
--rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.3/deepsecrets/core/model/rules/hashed_secret.py
--rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.3/deepsecrets/core/model/rules/hashing.py
--rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.3/deepsecrets/core/model/rules/regex.py
--rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.3/deepsecrets/core/model/rules/rule.py
--rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.3/deepsecrets/core/model/rules/semantic.py
--rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.3/deepsecrets/core/model/semantic.py
--rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.3/deepsecrets/core/model/token.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/core/modes/.DS_Store
--rw-r--r--   0        0        0     8546 2023-04-27 13:30:58.176068 deepsecrets-1.0.3/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
--rw-r--r--   0        0        0     5137 2023-04-27 13:30:57.438652 deepsecrets-1.0.3/deepsecrets/core/modes/iscan_mode.py
--rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
--rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
--rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
--rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
--rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
--rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
--rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
--rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
--rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
--rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
--rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
--rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/excluded_paths.py
--rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.3/deepsecrets/core/rulesets/false_findings.py
--rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.3/deepsecrets/core/rulesets/hashed_secrets.py
--rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/ibuilder.py
--rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.3/deepsecrets/core/rulesets/regex.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/.DS_Store
--rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__init__.py
--rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
--rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
--rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
--rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
--rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
--rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
--rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9685 2023-03-27 20:23:09.189108 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
--rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
--rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
--rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
--rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
--rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
--rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/full_content.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     3570 2023-04-14 12:50:43.000351 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
--rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
--rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
--rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/language.py
--rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
--rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
--rw-r--r--   0        0        0     6476 2023-04-14 13:10:20.748746 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
--rw-r--r--   0        0        0     5781 2023-04-14 13:10:20.026707 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
--rw-r--r--   0        0        0     2027 2023-04-14 12:50:42.345036 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/spot_improvements.py
--rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/type_stream.py
--rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.3/deepsecrets/core/tokenizers/itokenizer.py
--rw-r--r--   0        0        0     6015 2023-03-27 20:23:08.303488 deepsecrets-1.0.3/deepsecrets/core/tokenizers/lexer.py
--rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.3/deepsecrets/core/tokenizers/per_line.py
--rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.3/deepsecrets/core/tokenizers/per_word.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/core/utils/.DS_Store
--rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.3/deepsecrets/core/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
--rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.3/deepsecrets/core/utils/exceptions.py
--rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.3/deepsecrets/core/utils/file_analyzer.py
--rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.3/deepsecrets/core/utils/fs.py
--rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.3/deepsecrets/core/utils/hashing.py
--rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.3/deepsecrets/rules/excluded_paths.json
--rw-r--r--   0        0        0     3990 2023-03-27 20:07:41.216976 deepsecrets-1.0.3/deepsecrets/rules/regexes.json
--rw-r--r--   0        0        0        2 2023-02-22 17:11:42.000000 deepsecrets-1.0.3/deepsecrets/rules/semantic.json
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.3/deepsecrets/scan_modes/.DS_Store
--rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.3/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.3/deepsecrets/scan_modes/cli.py
--rw-r--r--   0        0        0     1666 2023-04-27 13:32:47.307536 deepsecrets-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 deepsecrets-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.0.4/README.md
+-rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.4/deepsecrets/.DS_Store
+-rw-r--r--   0        0        0      674 2023-04-27 13:31:17.046975 deepsecrets-1.0.4/deepsecrets/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.0.4/deepsecrets/__main__.py
+-rw-r--r--   0        0        0     6429 2023-04-28 06:49:11.562918 deepsecrets-1.0.4/deepsecrets/cli.py
+-rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.4/deepsecrets/config.py
+-rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/.DS_Store
+-rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.4/deepsecrets/core/engines/__init__.py
+-rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-04-17 13:35:10.334351 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     6184 2023-04-14 12:59:29.927306 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.4/deepsecrets/core/engines/hashed_secret.py
+-rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.4/deepsecrets/core/engines/iengine.py
+-rw-r--r--   0        0        0     1196 2023-04-17 13:35:09.681785 deepsecrets-1.0.4/deepsecrets/core/engines/regex.py
+-rw-r--r--   0        0        0     4333 2023-04-14 12:59:29.251562 deepsecrets-1.0.4/deepsecrets/core/engines/semantic.py
+-rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
+-rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
+-rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/content_analyzer.py
+-rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.4/deepsecrets/core/helpers/entropy.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/model/.DS_Store
+-rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.4/deepsecrets/core/model/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6910 2023-04-14 13:22:42.127475 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
+-rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     3719 2023-04-14 13:22:41.393440 deepsecrets-1.0.4/deepsecrets/core/model/file.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.4/deepsecrets/core/model/finding.py
+-rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/__init__.py
+-rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
+-rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/exlcuded_path.py
+-rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.4/deepsecrets/core/model/rules/false_finding.py
+-rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.4/deepsecrets/core/model/rules/hashed_secret.py
+-rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.4/deepsecrets/core/model/rules/hashing.py
+-rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.4/deepsecrets/core/model/rules/regex.py
+-rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.4/deepsecrets/core/model/rules/rule.py
+-rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/semantic.py
+-rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.4/deepsecrets/core/model/semantic.py
+-rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.4/deepsecrets/core/model/token.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/modes/.DS_Store
+-rw-r--r--   0        0        0     8425 2023-06-13 10:12:51.339833 deepsecrets-1.0.4/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
+-rw-r--r--   0        0        0     5157 2023-06-13 10:12:50.784613 deepsecrets-1.0.4/deepsecrets/core/modes/iscan_mode.py
+-rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
+-rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
+-rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
+-rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
+-rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
+-rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
+-rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
+-rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
+-rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
+-rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/excluded_paths.py
+-rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.4/deepsecrets/core/rulesets/false_findings.py
+-rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.4/deepsecrets/core/rulesets/hashed_secrets.py
+-rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/ibuilder.py
+-rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/regex.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/.DS_Store
+-rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
+-rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
+-rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
+-rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     9685 2023-03-27 20:23:09.189108 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
+-rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
+-rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
+-rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
+-rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/full_content.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     3570 2023-04-14 12:50:43.000351 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
+-rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
+-rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
+-rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/language.py
+-rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
+-rw-r--r--   0        0        0     6476 2023-04-14 13:10:20.748746 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
+-rw-r--r--   0        0        0     5781 2023-04-14 13:10:20.026707 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
+-rw-r--r--   0        0        0     2027 2023-04-14 12:50:42.345036 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/spot_improvements.py
+-rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/type_stream.py
+-rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/itokenizer.py
+-rw-r--r--   0        0        0     6015 2023-03-27 20:23:08.303488 deepsecrets-1.0.4/deepsecrets/core/tokenizers/lexer.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_line.py
+-rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_word.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
+-rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.4/deepsecrets/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.4/deepsecrets/core/utils/file_analyzer.py
+-rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.4/deepsecrets/core/utils/fs.py
+-rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.4/deepsecrets/core/utils/hashing.py
+-rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.4/deepsecrets/rules/excluded_paths.json
+-rw-r--r--   0        0        0     3990 2023-03-27 20:07:41.216976 deepsecrets-1.0.4/deepsecrets/rules/regexes.json
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/scan_modes/.DS_Store
+-rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.4/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.4/deepsecrets/scan_modes/cli.py
+-rw-r--r--   0        0        0     1666 2023-06-13 10:15:09.562204 deepsecrets-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 deepsecrets-1.0.4/PKG-INFO
```

### Comparing `deepsecrets-1.0.3/LICENSE` & `deepsecrets-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/README.md` & `deepsecrets-1.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 ## Yet another tool - why?
 Existing tools don't really "understand" code. Instead, they mostly parse texts.
 
 DeepSecrets expands classic regex-search approaches with semantic analysis, dangerous variable detection, and more efficient usage of entropy analysis. Code understanding supports 500+ languages and formats and is achieved by lexing and parsing - techniques commonly used in SAST tools.
 
 DeepSecrets also introduces a new way to find secrets: just use hashed values of your known secrets and get them found plain in your code.
 
+Under the hood story is in articles here: https://hackernoon.com/modernizing-secrets-scanning-part-1-the-problem 
+
+## Mini-FAQ after release :)
+> Pff, is it still regex-based?
+
+Yes and no. Of course, it uses regexes and finds typed secrets like any other tool. But language understanding (the lexing stage) and variable detection also use regexes under the hood. So regexes is an instrument, not a problem.
+
+> Why don't you build true abstract syntax trees? It's academically more correct!
+
+DeepSecrets tries to keep a balance between complexity and effectiveness. Building a true AST is a pretty complex thing and simply an overkill for our specific task. So the tool still follows the generic SAST-way of code analysis but optimizes the AST part using a different approach.
+
+> I'd like to build my own semantic rules. How do I do that?
+
+Only through the code by the moment. Formalizing the rules and moving them into a flexible and user-controlled ruleset is in the plans.
+
+> I still have a question
+
+Feel free to communicate with the [maintainer](https://github.com/avito-tech/deepsecrets/blob/main/pyproject.toml#L6-L8)
 
 ## Installation
 
 From Github via pip
 
 `$ pip install git+https://github.com/avito-tech/deepsecrets.git`
```

### Comparing `deepsecrets-1.0.3/deepsecrets/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/__init__.py` & `deepsecrets-1.0.4/deepsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/cli.py` & `deepsecrets-1.0.4/deepsecrets/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/config.py` & `deepsecrets-1.0.4/deepsecrets/config.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/hashed_secret.py` & `deepsecrets-1.0.4/deepsecrets/core/engines/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/iengine.py` & `deepsecrets-1.0.4/deepsecrets/core/engines/iengine.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/regex.py` & `deepsecrets-1.0.4/deepsecrets/core/engines/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/engines/semantic.py` & `deepsecrets-1.0.4/deepsecrets/core/engines/semantic.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/helpers/content_analyzer.py` & `deepsecrets-1.0.4/deepsecrets/core/helpers/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/helpers/entropy.py` & `deepsecrets-1.0.4/deepsecrets/core/helpers/entropy.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/core/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/file.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/__pycache__/token.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/token.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/file.py` & `deepsecrets-1.0.4/deepsecrets/core/model/file.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/finding.py` & `deepsecrets-1.0.4/deepsecrets/core/model/finding.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/rules/hashed_secret.py` & `deepsecrets-1.0.4/deepsecrets/core/model/rules/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/rules/regex.py` & `deepsecrets-1.0.4/deepsecrets/core/model/rules/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/rules/rule.py` & `deepsecrets-1.0.4/deepsecrets/core/model/rules/rule.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/model/token.py` & `deepsecrets-1.0.4/deepsecrets/core/model/token.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/modes/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/core/modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x11794a64 (Thu Apr 27 13:30:57 2023 UTC)
-files sz: 5137
+moddate:  0x22418864 (Tue Jun 13 10:12:50 2023 UTC)
+files sz: 5157
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -484,31 +484,28 @@
                   0x970067007d017c00a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d027c00a001000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007d037c0364
                   016b020000000072027c01530074040000000000000000000072347c006a
                   03000000000000000044005d2b7d047c01a0040000000000000000000000
                   0000000000000000007c00a0050000000000000000000000000000000000
                   0000007c04ac02a6010000ab010000000000000000a6010000ab01000000
-                  000000000001008c2c6eb47c00a006000000000000000000000000000000
+                  000000000001008c2c6e8c7c00a006000000000000000000000000000000
                   00000000007c03ac03a6010000ab01000000000000000035007d057c05a0
                   070000000000000000000000000000000000000000741100000000000000
                   0000007412000000000000000000007c027c006a050000000000000000a6
                   030000ab0300000000000000007c006a030000000000000000a6020000ab
-                  0200000000000000007d067c05a00a000000000000000000000000000000
-                  0000000000a6000000ab00000000000000000001007c05a00b0000000000
-                  000000000000000000000000000000a6000000ab00000000000000000001
-                  00640064006400a6020000ab02000000000000000001006e0b2300310073
-                  04770278035900770101005900010001007419000000000000000000007c
-                  06a6010000ab01000000000000000044005d1a7d077c0773018c057c01a0
-                  0400000000000000000000000000000000000000007c07a6010000ab0100
-                  0000000000000001008c1b741b000000000000000000007c01a6010000ab
-                  010000000000000000a00e00000000000000000000000000000000000000
-                  00a6000000ab0000000000000000007d087c00a00f000000000000000000
-                  00000000000000000000007c08a6010000ab0100000000000000007d087c
-                  085300
+                  0200000000000000007d06640064006400a6020000ab0200000000000000
+                  0001006e0b23003100730477027803590077010100590001000100741500
+                  0000000000000000007c06a6010000ab01000000000000000044005d1a7d
+                  077c0773018c057c01a00400000000000000000000000000000000000000
+                  007c07a6010000ab01000000000000000001008c1b741700000000000000
+                  0000007c01a6010000ab010000000000000000a00c000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000007d087c00a0
+                  0d00000000000000000000000000000000000000007c08a6010000ab0100
+                  000000000000007d087c085300
                 49           0 RESUME                   0
                
                 50           2 BUILD_LIST               0
                              4 STORE_FAST               1 (final)
                
                 52           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (analyzer_bundle)
@@ -548,15 +545,15 @@
                            186 PRECALL                  1
                            190 CALL                     1
                            200 PRECALL                  1
                            204 CALL                     1
                            214 POP_TOP
                            216 JUMP_BACKWARD           44 (to 130)
                
-                58     >>  218 JUMP_FORWARD           180 (to 580)
+                58     >>  218 JUMP_FORWARD           140 (to 500)
                
                 61     >>  220 LOAD_FAST                0 (self)
                            222 LOAD_METHOD              6 (pool_engine)
                            244 LOAD_FAST                3 (proc_count)
                            246 KW_NAMES                 3
                            248 PRECALL                  1
                            252 CALL                     1
@@ -577,103 +574,91 @@
                 64         342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR                3 (filepaths)
                
                 62         354 PRECALL                  2
                            358 CALL                     2
                            368 STORE_FAST               6 (per_file_findings)
                
-                67         370 LOAD_FAST                5 (pool)
-                           372 LOAD_METHOD             10 (close)
-                           394 PRECALL                  0
-                           398 CALL                     0
-                           408 POP_TOP
-               
-                68         410 LOAD_FAST                5 (pool)
-                           412 LOAD_METHOD             11 (join)
-                           434 PRECALL                  0
-                           438 CALL                     0
-                           448 POP_TOP
-               
-                61         450 LOAD_CONST               0 (None)
-                           452 LOAD_CONST               0 (None)
-                           454 LOAD_CONST               0 (None)
-                           456 PRECALL                  2
-                           460 CALL                     2
-                           470 POP_TOP
-                           472 JUMP_FORWARD            11 (to 496)
-                       >>  474 PUSH_EXC_INFO
-                           476 WITH_EXCEPT_START
-                           478 POP_JUMP_FORWARD_IF_TRUE     4 (to 488)
-                           480 RERAISE                  2
-                       >>  482 COPY                     3
-                           484 POP_EXCEPT
-                           486 RERAISE                  1
-                       >>  488 POP_TOP
-                           490 POP_EXCEPT
-                           492 POP_TOP
-                           494 POP_TOP
-               
-                70     >>  496 LOAD_GLOBAL             25 (NULL + list)
-                           508 LOAD_FAST                6 (per_file_findings)
-                           510 PRECALL                  1
-                           514 CALL                     1
-                           524 GET_ITER
-                       >>  526 FOR_ITER                26 (to 580)
-                           528 STORE_FAST               7 (file_findings)
-               
-                71         530 LOAD_FAST                7 (file_findings)
-                           532 POP_JUMP_FORWARD_IF_TRUE     1 (to 536)
-               
-                72         534 JUMP_BACKWARD            5 (to 526)
-               
-                73     >>  536 LOAD_FAST                1 (final)
-                           538 LOAD_METHOD              4 (extend)
-                           560 LOAD_FAST                7 (file_findings)
-                           562 PRECALL                  1
-                           566 CALL                     1
-                           576 POP_TOP
-                           578 JUMP_BACKWARD           27 (to 526)
-               
-                75     >>  580 LOAD_GLOBAL             27 (NULL + FindingMerger)
-                           592 LOAD_FAST                1 (final)
-                           594 PRECALL                  1
-                           598 CALL                     1
-                           608 LOAD_METHOD             14 (merge)
-                           630 PRECALL                  0
-                           634 CALL                     0
-                           644 STORE_FAST               8 (fin)
-               
-                76         646 LOAD_FAST                0 (self)
-                           648 LOAD_METHOD             15 (filter_false_positives)
-                           670 LOAD_FAST                8 (fin)
-                           672 PRECALL                  1
-                           676 CALL                     1
-                           686 STORE_FAST               8 (fin)
+                61         370 LOAD_CONST               0 (None)
+                           372 LOAD_CONST               0 (None)
+                           374 LOAD_CONST               0 (None)
+                           376 PRECALL                  2
+                           380 CALL                     2
+                           390 POP_TOP
+                           392 JUMP_FORWARD            11 (to 416)
+                       >>  394 PUSH_EXC_INFO
+                           396 WITH_EXCEPT_START
+                           398 POP_JUMP_FORWARD_IF_TRUE     4 (to 408)
+                           400 RERAISE                  2
+                       >>  402 COPY                     3
+                           404 POP_EXCEPT
+                           406 RERAISE                  1
+                       >>  408 POP_TOP
+                           410 POP_EXCEPT
+                           412 POP_TOP
+                           414 POP_TOP
+               
+                70     >>  416 LOAD_GLOBAL             21 (NULL + list)
+                           428 LOAD_FAST                6 (per_file_findings)
+                           430 PRECALL                  1
+                           434 CALL                     1
+                           444 GET_ITER
+                       >>  446 FOR_ITER                26 (to 500)
+                           448 STORE_FAST               7 (file_findings)
+               
+                71         450 LOAD_FAST                7 (file_findings)
+                           452 POP_JUMP_FORWARD_IF_TRUE     1 (to 456)
+               
+                72         454 JUMP_BACKWARD            5 (to 446)
+               
+                73     >>  456 LOAD_FAST                1 (final)
+                           458 LOAD_METHOD              4 (extend)
+                           480 LOAD_FAST                7 (file_findings)
+                           482 PRECALL                  1
+                           486 CALL                     1
+                           496 POP_TOP
+                           498 JUMP_BACKWARD           27 (to 446)
+               
+                75     >>  500 LOAD_GLOBAL             23 (NULL + FindingMerger)
+                           512 LOAD_FAST                1 (final)
+                           514 PRECALL                  1
+                           518 CALL                     1
+                           528 LOAD_METHOD             12 (merge)
+                           550 PRECALL                  0
+                           554 CALL                     0
+                           564 STORE_FAST               8 (fin)
+               
+                76         566 LOAD_FAST                0 (self)
+                           568 LOAD_METHOD             13 (filter_false_positives)
+                           590 LOAD_FAST                8 (fin)
+                           592 PRECALL                  1
+                           596 CALL                     1
+                           606 STORE_FAST               8 (fin)
                
-                77         688 LOAD_FAST                8 (fin)
-                           690 RETURN_VALUE
+                77         608 LOAD_FAST                8 (fin)
+                           610 RETURN_VALUE
                ExceptionTable:
-                 264 to 448 -> 474 [1] lasti
-                 474 to 480 -> 482 [3] lasti
-                 488 to 488 -> 482 [3] lasti
+                 264 to 368 -> 394 [1] lasti
+                 394 to 400 -> 402 [3] lasti
+                 408 to 408 -> 402 [3] lasti
                consts
                   None
                   0
                   ('file',)
                   ('processes',)
-               names      ('analyzer_bundle', '_get_process_count_for_runner', 'PROFILER_ON', 'filepaths', 'extend', '_per_file_analyzer', 'pool_engine', 'map', 'partial', 'pool_wrapper', 'close', 'join', 'list', 'FindingMerger', 'merge', 'filter_false_positives')
+               names      ('analyzer_bundle', '_get_process_count_for_runner', 'PROFILER_ON', 'filepaths', 'extend', '_per_file_analyzer', 'pool_engine', 'map', 'partial', 'pool_wrapper', 'list', 'FindingMerger', 'merge', 'filter_false_positives')
                varnames   ('self', 'final', 'bundle', 'proc_count', 'file', 'pool', 'per_file_findings', 'file_findings', 'fin')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       'run'
                firstlineno 49
                lnotab
                   0x02010402280128010c0104020e01120154ff02032e01180134010cfe10
-                  05280128f92e092201040102012c0242012a01
+                  ff2e092201040102012c0242012a01
             code
                argcount  : 1
                nlocals   : 10
                stacksize : 6
                flags     : 3
                code
                   0x970067007d017c006a000000000000000000733e740300000000000000
```

### Comparing `deepsecrets-1.0.3/deepsecrets/core/modes/iscan_mode.py` & `deepsecrets-1.0.4/deepsecrets/core/modes/iscan_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,17 @@
                 final.extend(self._per_file_analyzer(file=file))
         else:
             with self.pool_engine(processes=proc_count) as pool:
                 per_file_findings: List[List[Finding]] = pool.map(
                     partial(pool_wrapper, bundle, self._per_file_analyzer),
                     self.filepaths,
                 )  # type: ignore
-
-                pool.close()
-                pool.join()  # not calling because of suprusingly big delays
+                
+                # pool.close()
+                # pool.join()  # not calling because of suprusingly big delays
 
             for file_findings in list(per_file_findings):
                 if not file_findings:
                     continue
                 final.extend(file_findings)
 
         fin = FindingMerger(final).merge()
```

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/hashed_secrets.py` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/hashed_secrets.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/rulesets/ibuilder.py` & `deepsecrets-1.0.4/deepsecrets/core/rulesets/ibuilder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/language.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/language.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/spot_improvements.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/spot_improvements.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/helpers/type_stream.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/type_stream.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/itokenizer.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/itokenizer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/lexer.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/lexer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/per_line.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_line.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/tokenizers/per_word.py` & `deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_word.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/core/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/file_analyzer.py` & `deepsecrets-1.0.4/deepsecrets/core/utils/file_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/fs.py` & `deepsecrets-1.0.4/deepsecrets/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/core/utils/hashing.py` & `deepsecrets-1.0.4/deepsecrets/core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/rules/excluded_paths.json` & `deepsecrets-1.0.4/deepsecrets/rules/excluded_paths.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/rules/regexes.json` & `deepsecrets-1.0.4/deepsecrets/rules/regexes.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/scan_modes/.DS_Store` & `deepsecrets-1.0.4/deepsecrets/scan_modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc` & `deepsecrets-1.0.4/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/deepsecrets/scan_modes/cli.py` & `deepsecrets-1.0.4/deepsecrets/scan_modes/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.3/pyproject.toml` & `deepsecrets-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsecrets"
-version = "1.0.3"
+version = "1.0.4"
 description = "A better tool for secrets search"
 license = "MIT"
 authors = [
   "Nikolai Khechumov <khechumov@gmail.com>",
 ]
 keywords = ["security", "secrets", "credentials", "scanning", "appsec"]
 packages = [{include = "deepsecrets"}]
```

### Comparing `deepsecrets-1.0.3/PKG-INFO` & `deepsecrets-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsecrets
-Version: 1.0.3
+Version: 1.0.4
 Summary: A better tool for secrets search
 License: MIT
 Keywords: security,secrets,credentials,scanning,appsec
 Author: Nikolai Khechumov
 Author-email: khechumov@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
@@ -33,14 +33,32 @@
 ## Yet another tool - why?
 Existing tools don't really "understand" code. Instead, they mostly parse texts.
 
 DeepSecrets expands classic regex-search approaches with semantic analysis, dangerous variable detection, and more efficient usage of entropy analysis. Code understanding supports 500+ languages and formats and is achieved by lexing and parsing - techniques commonly used in SAST tools.
 
 DeepSecrets also introduces a new way to find secrets: just use hashed values of your known secrets and get them found plain in your code.
 
+Under the hood story is in articles here: https://hackernoon.com/modernizing-secrets-scanning-part-1-the-problem 
+
+## Mini-FAQ after release :)
+> Pff, is it still regex-based?
+
+Yes and no. Of course, it uses regexes and finds typed secrets like any other tool. But language understanding (the lexing stage) and variable detection also use regexes under the hood. So regexes is an instrument, not a problem.
+
+> Why don't you build true abstract syntax trees? It's academically more correct!
+
+DeepSecrets tries to keep a balance between complexity and effectiveness. Building a true AST is a pretty complex thing and simply an overkill for our specific task. So the tool still follows the generic SAST-way of code analysis but optimizes the AST part using a different approach.
+
+> I'd like to build my own semantic rules. How do I do that?
+
+Only through the code by the moment. Formalizing the rules and moving them into a flexible and user-controlled ruleset is in the plans.
+
+> I still have a question
+
+Feel free to communicate with the [maintainer](https://github.com/avito-tech/deepsecrets/blob/main/pyproject.toml#L6-L8)
 
 ## Installation
 
 From Github via pip
 
 `$ pip install git+https://github.com/avito-tech/deepsecrets.git`
```

