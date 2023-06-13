# Comparing `tmp/garak-0.9.tar.gz` & `tmp/garak-0.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garak-0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "garak-0.9.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `garak-0.9.tar` & `garak-0.9.post1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     3112 2023-06-06 16:45:01.347727 garak-0.9/.gitignore
--rw-r--r--   0        0        0     2589 2023-06-12 21:52:09.620252 garak-0.9/FAQ.md
--rw-r--r--   0        0        0    35148 2023-06-06 16:45:01.351727 garak-0.9/LICENSE
--rw-r--r--   0        0        0    11779 2023-06-12 21:51:02.458027 garak-0.9/README.md
--rw-r--r--   0        0        0     2127 2023-06-09 04:26:49.000000 garak-0.9/analyse/analyse_log.py
--rw-r--r--   0        0        0      103 2023-06-06 16:45:01.351727 garak-0.9/garak/__init__.py
--rw-r--r--   0        0        0      147 2023-06-06 16:45:01.351727 garak-0.9/garak/__main__.py
--rw-r--r--   0        0        0       65 2023-06-06 16:45:01.351727 garak-0.9/garak/_config.py
--rw-r--r--   0        0        0     4276 2023-06-12 21:04:16.178398 garak-0.9/garak/_plugins.py
--rw-r--r--   0        0        0      989 2023-06-06 16:45:01.351727 garak-0.9/garak/attempt.py
--rw-r--r--   0        0        0     8967 2023-06-09 05:48:04.000000 garak-0.9/garak/cli.py
--rw-r--r--   0        0        0       20 2023-05-25 19:31:38.000000 garak-0.9/garak/detectors/__init__.py
--rw-r--r--   0        0        0      473 2023-06-12 16:17:14.121260 garak-0.9/garak/detectors/always.py
--rw-r--r--   0        0        0     4636 2023-06-12 18:50:39.000000 garak-0.9/garak/detectors/base.py
--rw-r--r--   0        0        0      893 2023-06-12 18:05:58.000000 garak-0.9/garak/detectors/continuation.py
--rw-r--r--   0        0        0     1819 2023-06-12 18:07:57.000000 garak-0.9/garak/detectors/dan.py
--rw-r--r--   0        0        0     1566 2023-06-12 18:10:23.000000 garak-0.9/garak/detectors/encoding.py
--rw-r--r--   0        0        0     2490 2023-06-12 18:13:28.000000 garak-0.9/garak/detectors/goodside.py
--rw-r--r--   0        0        0      926 2023-06-12 18:05:04.000000 garak-0.9/garak/detectors/knownbadsignatures.py
--rw-r--r--   0        0        0      949 2023-06-12 21:14:54.258359 garak-0.9/garak/detectors/lmrc.py
--rw-r--r--   0        0        0     3455 2023-06-12 16:30:32.946011 garak-0.9/garak/detectors/misleading.py
--rw-r--r--   0        0        0     4545 2023-06-12 16:30:32.938011 garak-0.9/garak/detectors/mitigation.py
--rw-r--r--   0        0        0     7188 2023-06-06 16:45:01.359728 garak-0.9/garak/detectors/perspective.py
--rw-r--r--   0        0        0      830 2023-06-12 16:26:26.179226 garak-0.9/garak/detectors/promptinject.py
--rw-r--r--   0        0        0     6075 2023-06-12 16:26:53.949519 garak-0.9/garak/detectors/riskywords.py
--rw-r--r--   0        0        0     1107 2023-06-12 16:19:39.058207 garak-0.9/garak/detectors/snowball.py
--rw-r--r--   0        0        0      666 2023-06-12 16:18:45.660695 garak-0.9/garak/detectors/specialwords.py
--rw-r--r--   0        0        0      476 2023-06-12 16:17:38.301750 garak-0.9/garak/detectors/toxicity.py
--rw-r--r--   0        0        0       20 2023-05-24 18:09:40.911631 garak-0.9/garak/evaluators/__init__.py
--rw-r--r--   0        0        0     2785 2023-06-09 05:46:41.000000 garak-0.9/garak/evaluators/base.py
--rw-r--r--   0        0        0      436 2023-06-06 16:45:01.359728 garak-0.9/garak/evaluators/maxrecall.py
--rw-r--r--   0        0        0       25 2023-06-06 16:45:01.363728 garak-0.9/garak/generators/__init__.py
--rw-r--r--   0        0        0      820 2023-06-12 20:36:47.604168 garak-0.9/garak/generators/base.py
--rw-r--r--   0        0        0     2796 2023-06-12 20:38:25.518748 garak-0.9/garak/generators/cohere.py
--rw-r--r--   0        0        0     1803 2023-06-12 20:59:20.721695 garak-0.9/garak/generators/ggml.py
--rw-r--r--   0        0        0     5659 2023-06-12 20:44:41.785963 garak-0.9/garak/generators/huggingface.py
--rw-r--r--   0        0        0     3591 2023-06-12 20:42:24.667729 garak-0.9/garak/generators/openai.py
--rw-r--r--   0        0        0     1866 2023-06-12 20:50:31.830375 garak-0.9/garak/generators/replicate.py
--rw-r--r--   0        0        0      368 2023-06-12 20:38:47.047267 garak-0.9/garak/generators/test.py
--rw-r--r--   0        0        0       20 2023-05-24 18:09:40.911631 garak-0.9/garak/harness/__init__.py
--rw-r--r--   0        0        0     2353 2023-06-06 18:09:15.499255 garak-0.9/garak/harness/base.py
--rw-r--r--   0        0        0     1626 2023-06-06 16:45:01.367728 garak-0.9/garak/harness/probewise.py
--rw-r--r--   0        0        0     1985 2023-06-06 18:09:15.499255 garak-0.9/garak/harness/pxd.py
--rw-r--r--   0        0        0       20 2023-05-24 18:09:40.915631 garak-0.9/garak/probes/__init__.py
--rw-r--r--   0        0        0     4419 2023-06-12 18:56:28.000000 garak-0.9/garak/probes/art.py
--rw-r--r--   0        0        0     2534 2023-06-12 22:20:40.493311 garak-0.9/garak/probes/base.py
--rw-r--r--   0        0        0      359 2023-06-12 15:47:06.457785 garak-0.9/garak/probes/blank.py
--rw-r--r--   0        0        0     2023 2023-06-12 18:05:49.000000 garak-0.9/garak/probes/continuation.py
--rw-r--r--   0        0        0    50910 2023-06-12 15:54:32.750009 garak-0.9/garak/probes/dan.py
--rw-r--r--   0        0        0    12703 2023-06-12 16:03:16.602807 garak-0.9/garak/probes/encoding.py
--rw-r--r--   0        0        0     3386 2023-06-12 16:04:24.018802 garak-0.9/garak/probes/goodside.py
--rw-r--r--   0        0        0     4420 2023-06-12 16:05:37.410863 garak-0.9/garak/probes/knownbadsignatures.py
--rw-r--r--   0        0        0     5924 2023-06-12 21:14:54.322360 garak-0.9/garak/probes/lmrc.py
--rw-r--r--   0        0        0     1157 2023-06-12 16:11:09.499782 garak-0.9/garak/probes/misleading.py
--rw-r--r--   0        0        0     3636 2023-06-06 21:47:36.106406 garak-0.9/garak/probes/promptinject.py
--rw-r--r--   0        0        0     2357 2023-06-12 15:56:25.652678 garak-0.9/garak/probes/realtoxicityprompts.py
--rw-r--r--   0        0        0     1446 2023-06-12 15:48:50.773794 garak-0.9/garak/probes/snowball.py
--rw-r--r--   0        0        0     1006 2023-06-12 22:43:07.741143 garak-0.9/pyproject.toml
--rw-r--r--   0        0        0      190 2023-06-08 23:24:41.736152 garak-0.9/requirements.txt
--rw-r--r--   0        0        0   344501 2023-06-06 16:45:01.379728 garak-0.9/resources/graph_connectivity.json
--rw-r--r--   0        0        0     3777 2023-06-06 16:45:01.379728 garak-0.9/resources/ldnoobw-en.txt
--rw-r--r--   0        0        0     2855 2023-06-06 16:45:01.379728 garak-0.9/resources/ofcom-potentially-offensive.txt
--rw-r--r--   0        0        0    37017 2023-06-06 16:45:01.379728 garak-0.9/resources/primality_testing.json
--rw-r--r--   0        0        0   105714 2023-06-06 16:45:01.379728 garak-0.9/resources/profanity_en.csv
--rw-r--r--   0        0        0      174 2023-06-06 21:41:52.182495 garak-0.9/resources/promptinject/__init__.py
--rw-r--r--   0        0        0      615 2023-06-06 21:41:52.182495 garak-0.9/resources/promptinject/_utils.py
--rw-r--r--   0        0        0    26965 2023-06-06 21:41:52.182495 garak-0.9/resources/promptinject/prompt_data.py
--rw-r--r--   0        0        0    10015 2023-06-06 21:41:52.182495 garak-0.9/resources/promptinject/prompting.py
--rw-r--r--   0        0        0     1836 2023-06-06 21:41:52.182495 garak-0.9/resources/promptinject/run.py
--rw-r--r--   0        0        0     2377 2023-06-06 21:41:52.186495 garak-0.9/resources/promptinject/scoring.py
--rw-r--r--   0        0        0     1343 2023-06-06 21:41:52.186495 garak-0.9/resources/promptinject/visualization.py
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.383728 garak-0.9/resources/rtp_flirtation.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.383728 garak-0.9/resources/rtp_identity_attack.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.383728 garak-0.9/resources/rtp_insult.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.383728 garak-0.9/resources/rtp_profanity.txt
--rw-r--r--   0        0        0     4454 2023-06-06 16:45:01.383728 garak-0.9/resources/rtp_severe_toxicity.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.383728 garak-0.9/resources/rtp_sexually_explicit.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.383728 garak-0.9/resources/rtp_threat.txt
--rw-r--r--   0        0        0    58554 2023-06-06 16:45:01.383728 garak-0.9/resources/senator_search.json
--rw-r--r--   0        0        0   152480 2023-06-06 18:09:15.503255 garak-0.9/resources/slurprompts.jsonl
--rw-r--r--   0        0        0     6836 2023-06-10 23:40:40.220566 garak-0.9/resources/slurprompts_80.jsonl
--rw-r--r--   0        0        0     5487 2023-06-06 16:45:01.391728 garak-0.9/resources/slursreclaimedslurs.txt
--rw-r--r--   0        0        0     1182 2023-06-06 16:45:01.391728 garak-0.9/resources/termscrape.py
--rw-r--r--   0        0        0   151324 2023-06-06 16:45:01.387728 garak-0.9/resources/truefalse_falseclaims.txt
--rw-r--r--   0        0        0     2389 2023-06-06 16:45:01.387728 garak-0.9/resources/truefalse_falseclaims_50.txt
--rw-r--r--   0        0        0     1656 2023-06-12 22:19:11.095885 garak-0.9/tests/test_cli.py
--rw-r--r--   0        0        0    12704 1970-01-01 00:00:00.000000 garak-0.9/PKG-INFO
+-rw-r--r--   0        0        0     3112 2023-06-06 16:45:01.000000 garak-0.9.post1/.gitignore
+-rw-r--r--   0        0        0     2589 2023-06-12 21:52:09.000000 garak-0.9.post1/FAQ.md
+-rw-r--r--   0        0        0    35148 2023-06-06 16:45:01.000000 garak-0.9.post1/LICENSE
+-rw-r--r--   0        0        0    11821 2023-06-12 22:58:08.000000 garak-0.9.post1/README.md
+-rw-r--r--   0        0        0     2127 2023-06-09 04:26:49.061116 garak-0.9.post1/analyse/analyse_log.py
+-rw-r--r--   0        0        0      109 2023-06-13 03:55:23.603339 garak-0.9.post1/garak/__init__.py
+-rw-r--r--   0        0        0      147 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/__main__.py
+-rw-r--r--   0        0        0       65 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/_config.py
+-rw-r--r--   0        0        0     4276 2023-06-12 21:04:16.000000 garak-0.9.post1/garak/_plugins.py
+-rw-r--r--   0        0        0      989 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/attempt.py
+-rw-r--r--   0        0        0     8967 2023-06-09 05:48:04.717785 garak-0.9.post1/garak/cli.py
+-rw-r--r--   0        0        0       20 2023-05-25 19:31:38.000000 garak-0.9.post1/garak/detectors/__init__.py
+-rw-r--r--   0        0        0      473 2023-06-12 16:17:04.000000 garak-0.9.post1/garak/detectors/always.py
+-rw-r--r--   0        0        0     4636 2023-06-12 18:50:46.127757 garak-0.9.post1/garak/detectors/base.py
+-rw-r--r--   0        0        0      893 2023-06-12 18:05:58.081058 garak-0.9.post1/garak/detectors/continuation.py
+-rw-r--r--   0        0        0     1819 2023-06-12 18:07:57.560004 garak-0.9.post1/garak/detectors/dan.py
+-rw-r--r--   0        0        0     1566 2023-06-12 18:10:36.242329 garak-0.9.post1/garak/detectors/encoding.py
+-rw-r--r--   0        0        0     2490 2023-06-12 18:13:28.210817 garak-0.9.post1/garak/detectors/goodside.py
+-rw-r--r--   0        0        0      926 2023-06-12 18:05:04.915540 garak-0.9.post1/garak/detectors/knownbadsignatures.py
+-rw-r--r--   0        0        0      949 2023-06-12 21:14:54.000000 garak-0.9.post1/garak/detectors/lmrc.py
+-rw-r--r--   0        0        0     3455 2023-06-12 16:30:32.000000 garak-0.9.post1/garak/detectors/misleading.py
+-rw-r--r--   0        0        0     4545 2023-06-12 16:30:32.000000 garak-0.9.post1/garak/detectors/mitigation.py
+-rw-r--r--   0        0        0     7188 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/detectors/perspective.py
+-rw-r--r--   0        0        0      830 2023-06-12 16:26:20.000000 garak-0.9.post1/garak/detectors/promptinject.py
+-rw-r--r--   0        0        0     6075 2023-06-12 16:26:53.000000 garak-0.9.post1/garak/detectors/riskywords.py
+-rw-r--r--   0        0        0     1107 2023-06-12 16:19:39.000000 garak-0.9.post1/garak/detectors/snowball.py
+-rw-r--r--   0        0        0      666 2023-06-12 16:18:45.000000 garak-0.9.post1/garak/detectors/specialwords.py
+-rw-r--r--   0        0        0      476 2023-06-12 16:17:38.000000 garak-0.9.post1/garak/detectors/toxicity.py
+-rw-r--r--   0        0        0       20 2023-05-18 03:08:10.893234 garak-0.9.post1/garak/evaluators/__init__.py
+-rw-r--r--   0        0        0     2785 2023-06-09 05:46:41.839174 garak-0.9.post1/garak/evaluators/base.py
+-rw-r--r--   0        0        0      436 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/evaluators/maxrecall.py
+-rw-r--r--   0        0        0       25 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/generators/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-12 20:36:47.000000 garak-0.9.post1/garak/generators/base.py
+-rw-r--r--   0        0        0     2796 2023-06-12 20:38:25.000000 garak-0.9.post1/garak/generators/cohere.py
+-rw-r--r--   0        0        0     1803 2023-06-12 20:59:20.000000 garak-0.9.post1/garak/generators/ggml.py
+-rw-r--r--   0        0        0     5659 2023-06-12 20:44:41.000000 garak-0.9.post1/garak/generators/huggingface.py
+-rw-r--r--   0        0        0     3591 2023-06-12 20:42:24.000000 garak-0.9.post1/garak/generators/openai.py
+-rw-r--r--   0        0        0     1866 2023-06-12 20:50:31.000000 garak-0.9.post1/garak/generators/replicate.py
+-rw-r--r--   0        0        0      368 2023-06-12 20:38:47.000000 garak-0.9.post1/garak/generators/test.py
+-rw-r--r--   0        0        0       20 2023-05-18 03:08:10.934500 garak-0.9.post1/garak/harness/__init__.py
+-rw-r--r--   0        0        0     2353 2023-06-06 18:09:15.000000 garak-0.9.post1/garak/harness/base.py
+-rw-r--r--   0        0        0     1626 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/harness/probewise.py
+-rw-r--r--   0        0        0     1985 2023-06-06 18:09:15.000000 garak-0.9.post1/garak/harness/pxd.py
+-rw-r--r--   0        0        0       20 2023-05-18 03:08:10.940450 garak-0.9.post1/garak/probes/__init__.py
+-rw-r--r--   0        0        0     4475 2023-06-13 03:50:04.172383 garak-0.9.post1/garak/probes/art.py
+-rw-r--r--   0        0        0     2534 2023-06-12 22:20:40.000000 garak-0.9.post1/garak/probes/base.py
+-rw-r--r--   0        0        0      359 2023-06-12 15:47:06.000000 garak-0.9.post1/garak/probes/blank.py
+-rw-r--r--   0        0        0     2023 2023-06-12 18:05:49.609069 garak-0.9.post1/garak/probes/continuation.py
+-rw-r--r--   0        0        0    50910 2023-06-12 15:54:28.000000 garak-0.9.post1/garak/probes/dan.py
+-rw-r--r--   0        0        0    12703 2023-06-12 16:03:16.000000 garak-0.9.post1/garak/probes/encoding.py
+-rw-r--r--   0        0        0     3386 2023-06-12 16:04:24.000000 garak-0.9.post1/garak/probes/goodside.py
+-rw-r--r--   0        0        0     4420 2023-06-12 16:05:37.000000 garak-0.9.post1/garak/probes/knownbadsignatures.py
+-rw-r--r--   0        0        0     5924 2023-06-12 21:14:54.000000 garak-0.9.post1/garak/probes/lmrc.py
+-rw-r--r--   0        0        0     1157 2023-06-12 16:11:09.000000 garak-0.9.post1/garak/probes/misleading.py
+-rw-r--r--   0        0        0     3636 2023-06-06 21:47:36.000000 garak-0.9.post1/garak/probes/promptinject.py
+-rw-r--r--   0        0        0     2357 2023-06-12 15:56:25.000000 garak-0.9.post1/garak/probes/realtoxicityprompts.py
+-rw-r--r--   0        0        0     1446 2023-06-12 15:48:50.000000 garak-0.9.post1/garak/probes/snowball.py
+-rw-r--r--   0        0        0     1002 2023-06-13 03:53:59.366505 garak-0.9.post1/pyproject.toml
+-rw-r--r--   0        0        0      185 2023-06-13 03:52:09.491824 garak-0.9.post1/requirements.txt
+-rw-r--r--   0        0        0   344501 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/graph_connectivity.json
+-rw-r--r--   0        0        0     3777 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/ldnoobw-en.txt
+-rw-r--r--   0        0        0     2855 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/ofcom-potentially-offensive.txt
+-rw-r--r--   0        0        0    37017 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/primality_testing.json
+-rw-r--r--   0        0        0   105714 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/profanity_en.csv
+-rw-r--r--   0        0        0      174 2023-06-06 20:59:34.000000 garak-0.9.post1/resources/promptinject/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/_utils.py
+-rw-r--r--   0        0        0    26965 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/prompt_data.py
+-rw-r--r--   0        0        0    10015 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/prompting.py
+-rw-r--r--   0        0        0     1836 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/run.py
+-rw-r--r--   0        0        0     2377 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/scoring.py
+-rw-r--r--   0        0        0     1343 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/visualization.py
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_flirtation.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_identity_attack.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_insult.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_profanity.txt
+-rw-r--r--   0        0        0     4454 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_severe_toxicity.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_sexually_explicit.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_threat.txt
+-rw-r--r--   0        0        0    58554 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/senator_search.json
+-rw-r--r--   0        0        0   152480 2023-06-06 18:09:15.000000 garak-0.9.post1/resources/slurprompts.jsonl
+-rw-r--r--   0        0        0     6836 2023-06-10 23:40:40.000000 garak-0.9.post1/resources/slurprompts_80.jsonl
+-rw-r--r--   0        0        0     5487 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/slursreclaimedslurs.txt
+-rw-r--r--   0        0        0     1182 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/termscrape.py
+-rw-r--r--   0        0        0   151324 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/truefalse_falseclaims.txt
+-rw-r--r--   0        0        0     2389 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/truefalse_falseclaims_50.txt
+-rw-r--r--   0        0        0     1656 2023-06-12 22:19:11.000000 garak-0.9.post1/tests/test_cli.py
+-rw-r--r--   0        0        0    12732 1970-01-01 00:00:00.000000 garak-0.9.post1/PKG-INFO
```

### Comparing `garak-0.9/.gitignore` & `garak-0.9.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `garak-0.9/FAQ.md` & `garak-0.9.post1/FAQ.md`

 * *Files identical despite different names*

### Comparing `garak-0.9/LICENSE` & `garak-0.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `garak-0.9/README.md` & `garak-0.9.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     * For detectors, try a blank generator and a blank probe: `python3 -m garak -m test.Blank -p blank -d mymodule`
     * For generators, try a blank probe and always.Pass detector: `python3 -m garak -m mymodule -p blank -d always.Pass`
   * Get `garak` to list all the plugins of the type you're writing, with `--list_probes`, `--list_detectors`, or `--list_generators`
 
 
 ## FAQ
 
-We have an FAQ [here](FAQ.md). Reach out if you have any more questions!
+We have an FAQ [here](https://github.com/leondz/garak/blob/main/FAQ.md). Reach out if you have any more questions!
 
 <hr>
 
 _"Never tell the same lie twice"_ - Elim
 
 
 © GPLv3 2023 Leon Derczynski
```

### Comparing `garak-0.9/analyse/analyse_log.py` & `garak-0.9.post1/analyse/analyse_log.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/_plugins.py` & `garak-0.9.post1/garak/_plugins.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/attempt.py` & `garak-0.9.post1/garak/attempt.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/cli.py` & `garak-0.9.post1/garak/cli.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/base.py` & `garak-0.9.post1/garak/detectors/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/continuation.py` & `garak-0.9.post1/garak/detectors/continuation.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/dan.py` & `garak-0.9.post1/garak/detectors/dan.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/encoding.py` & `garak-0.9.post1/garak/detectors/encoding.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/goodside.py` & `garak-0.9.post1/garak/detectors/goodside.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/knownbadsignatures.py` & `garak-0.9.post1/garak/detectors/knownbadsignatures.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/lmrc.py` & `garak-0.9.post1/garak/detectors/lmrc.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/misleading.py` & `garak-0.9.post1/garak/detectors/misleading.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/mitigation.py` & `garak-0.9.post1/garak/detectors/mitigation.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/perspective.py` & `garak-0.9.post1/garak/detectors/perspective.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/promptinject.py` & `garak-0.9.post1/garak/detectors/promptinject.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/riskywords.py` & `garak-0.9.post1/garak/detectors/riskywords.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/snowball.py` & `garak-0.9.post1/garak/detectors/snowball.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/detectors/specialwords.py` & `garak-0.9.post1/garak/detectors/specialwords.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/evaluators/base.py` & `garak-0.9.post1/garak/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/generators/base.py` & `garak-0.9.post1/garak/generators/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/generators/cohere.py` & `garak-0.9.post1/garak/generators/cohere.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/generators/ggml.py` & `garak-0.9.post1/garak/generators/ggml.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/generators/huggingface.py` & `garak-0.9.post1/garak/generators/huggingface.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/generators/openai.py` & `garak-0.9.post1/garak/generators/openai.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/generators/replicate.py` & `garak-0.9.post1/garak/generators/replicate.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/harness/base.py` & `garak-0.9.post1/garak/harness/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/harness/probewise.py` & `garak-0.9.post1/garak/harness/probewise.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/harness/pxd.py` & `garak-0.9.post1/garak/harness/pxd.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/art.py` & `garak-0.9.post1/garak/probes/art.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     description = "Auto Red-Team"
     recommended_detector = ["toxicity.ToxicCommentModel"]
     redteamer = None
     max_calls = 5
     constructive_tension = True
 
     def __init__(self):
-        import nltk
-
         super().__init__()
 
     def probe(self, generator) -> List[garak.attempt.Attempt]:
         if self.redteamer == None:
             self.redteamer = Local("leondz/artgpt2tox")
             self.redteamer.generations = 1
             self.redteamer.deprefix_prompt = True
@@ -65,15 +63,17 @@
 
             while calls_made < self.max_calls and keep_going:
                 # generate a challenge
                 if last_response == "" and self.constructive_tension:
                     challenge = ""
                 else:
                     if last_response:
-                        last_response_first_sent = nltk.sent_tokenize(last_response)[0]
+                        last_response_first_sent = last_response.split(". ")[
+                            0
+                        ]  # nltk install too unfriendly
                     else:
                         last_response_first_sent = ""
 
                     query = f"<|input|>{last_response_first_sent}<|response|>"
                     # print("query:", query)
                     challenge = self.redteamer.generate(query)
                     # print("challenge:", challenge)
```

### Comparing `garak-0.9/garak/probes/base.py` & `garak-0.9.post1/garak/probes/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/continuation.py` & `garak-0.9.post1/garak/probes/continuation.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/dan.py` & `garak-0.9.post1/garak/probes/dan.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/encoding.py` & `garak-0.9.post1/garak/probes/encoding.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/goodside.py` & `garak-0.9.post1/garak/probes/goodside.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/knownbadsignatures.py` & `garak-0.9.post1/garak/probes/knownbadsignatures.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/lmrc.py` & `garak-0.9.post1/garak/probes/lmrc.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/misleading.py` & `garak-0.9.post1/garak/probes/misleading.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/promptinject.py` & `garak-0.9.post1/garak/probes/promptinject.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/realtoxicityprompts.py` & `garak-0.9.post1/garak/probes/realtoxicityprompts.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/garak/probes/snowball.py` & `garak-0.9.post1/garak/probes/snowball.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/pyproject.toml` & `garak-0.9.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "garak"
-version = "0.9"
+version = "0.9.post1"
 authors = [
   { name= "Leon Derczynski", email="leonderczynski@gmail.com" },
 ]
 license = { file = "LICENSE" }
 description = "LLM vulnerability scanner"
 readme = "README.md"
 classifiers = [
@@ -27,15 +27,14 @@
   "cohere>=4.5.1",
   "openai>=0.27.7",
   "replicate>=0.8.3",
   "pytest>=7.3",
   "google-api-python-client>=2.0",
   "backoff>=2.1.1",
   "torch",
-  "nltk",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/leondz/garak"
 "Bug Tracker" = "https://github.com/leondz/garak/issues"
 
 [project.scripts]
```

### Comparing `garak-0.9/resources/graph_connectivity.json` & `garak-0.9.post1/resources/graph_connectivity.json`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/ldnoobw-en.txt` & `garak-0.9.post1/resources/ldnoobw-en.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/ofcom-potentially-offensive.txt` & `garak-0.9.post1/resources/ofcom-potentially-offensive.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/primality_testing.json` & `garak-0.9.post1/resources/primality_testing.json`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/profanity_en.csv` & `garak-0.9.post1/resources/profanity_en.csv`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/promptinject/_utils.py` & `garak-0.9.post1/resources/promptinject/_utils.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/promptinject/prompt_data.py` & `garak-0.9.post1/resources/promptinject/prompt_data.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/promptinject/prompting.py` & `garak-0.9.post1/resources/promptinject/prompting.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/promptinject/run.py` & `garak-0.9.post1/resources/promptinject/run.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/promptinject/scoring.py` & `garak-0.9.post1/resources/promptinject/scoring.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/promptinject/visualization.py` & `garak-0.9.post1/resources/promptinject/visualization.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/rtp_flirtation.txt` & `garak-0.9.post1/resources/rtp_flirtation.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/rtp_identity_attack.txt` & `garak-0.9.post1/resources/rtp_identity_attack.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/rtp_insult.txt` & `garak-0.9.post1/resources/rtp_insult.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/rtp_profanity.txt` & `garak-0.9.post1/resources/rtp_profanity.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/rtp_severe_toxicity.txt` & `garak-0.9.post1/resources/rtp_severe_toxicity.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/rtp_sexually_explicit.txt` & `garak-0.9.post1/resources/rtp_sexually_explicit.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/rtp_threat.txt` & `garak-0.9.post1/resources/rtp_threat.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/senator_search.json` & `garak-0.9.post1/resources/senator_search.json`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/slurprompts.jsonl` & `garak-0.9.post1/resources/slurprompts.jsonl`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/slurprompts_80.jsonl` & `garak-0.9.post1/resources/slurprompts_80.jsonl`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/slursreclaimedslurs.txt` & `garak-0.9.post1/resources/slursreclaimedslurs.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/termscrape.py` & `garak-0.9.post1/resources/termscrape.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/truefalse_falseclaims.txt` & `garak-0.9.post1/resources/truefalse_falseclaims.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/resources/truefalse_falseclaims_50.txt` & `garak-0.9.post1/resources/truefalse_falseclaims_50.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9/tests/test_cli.py` & `garak-0.9.post1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `garak-0.9/PKG-INFO` & `garak-0.9.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garak
-Version: 0.9
+Version: 0.9.post1
 Summary: LLM vulnerability scanner
 Author-email: Leon Derczynski <leonderczynski@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,14 @@
 Requires-Dist: cohere>=4.5.1
 Requires-Dist: openai>=0.27.7
 Requires-Dist: replicate>=0.8.3
 Requires-Dist: pytest>=7.3
 Requires-Dist: google-api-python-client>=2.0
 Requires-Dist: backoff>=2.1.1
 Requires-Dist: torch
-Requires-Dist: nltk
 Project-URL: Bug Tracker, https://github.com/leondz/garak/issues
 Project-URL: Homepage, https://github.com/leondz/garak
 
 # garak, an llm vulnerability scanner
 
 `garak` is a modular tool for probing LLMs for undesireable prompt responses
 
@@ -252,15 +251,15 @@
     * For detectors, try a blank generator and a blank probe: `python3 -m garak -m test.Blank -p blank -d mymodule`
     * For generators, try a blank probe and always.Pass detector: `python3 -m garak -m mymodule -p blank -d always.Pass`
   * Get `garak` to list all the plugins of the type you're writing, with `--list_probes`, `--list_detectors`, or `--list_generators`
 
 
 ## FAQ
 
-We have an FAQ [here](FAQ.md). Reach out if you have any more questions!
+We have an FAQ [here](https://github.com/leondz/garak/blob/main/FAQ.md). Reach out if you have any more questions!
 
 <hr>
 
 _"Never tell the same lie twice"_ - Elim
 
 
 © GPLv3 2023 Leon Derczynski
```

