# Comparing `tmp/garak-0.9.post1.tar.gz` & `tmp/garak-0.9.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garak-0.9.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "garak-0.9.post2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `garak-0.9.post1.tar` & `garak-0.9.post2.tar`

### file list

```diff
@@ -1,87 +1,89 @@
--rw-r--r--   0        0        0     3112 2023-06-06 16:45:01.000000 garak-0.9.post1/.gitignore
--rw-r--r--   0        0        0     2589 2023-06-12 21:52:09.000000 garak-0.9.post1/FAQ.md
--rw-r--r--   0        0        0    35148 2023-06-06 16:45:01.000000 garak-0.9.post1/LICENSE
--rw-r--r--   0        0        0    11821 2023-06-12 22:58:08.000000 garak-0.9.post1/README.md
--rw-r--r--   0        0        0     2127 2023-06-09 04:26:49.061116 garak-0.9.post1/analyse/analyse_log.py
--rw-r--r--   0        0        0      109 2023-06-13 03:55:23.603339 garak-0.9.post1/garak/__init__.py
--rw-r--r--   0        0        0      147 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/__main__.py
--rw-r--r--   0        0        0       65 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/_config.py
--rw-r--r--   0        0        0     4276 2023-06-12 21:04:16.000000 garak-0.9.post1/garak/_plugins.py
--rw-r--r--   0        0        0      989 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/attempt.py
--rw-r--r--   0        0        0     8967 2023-06-09 05:48:04.717785 garak-0.9.post1/garak/cli.py
--rw-r--r--   0        0        0       20 2023-05-25 19:31:38.000000 garak-0.9.post1/garak/detectors/__init__.py
--rw-r--r--   0        0        0      473 2023-06-12 16:17:04.000000 garak-0.9.post1/garak/detectors/always.py
--rw-r--r--   0        0        0     4636 2023-06-12 18:50:46.127757 garak-0.9.post1/garak/detectors/base.py
--rw-r--r--   0        0        0      893 2023-06-12 18:05:58.081058 garak-0.9.post1/garak/detectors/continuation.py
--rw-r--r--   0        0        0     1819 2023-06-12 18:07:57.560004 garak-0.9.post1/garak/detectors/dan.py
--rw-r--r--   0        0        0     1566 2023-06-12 18:10:36.242329 garak-0.9.post1/garak/detectors/encoding.py
--rw-r--r--   0        0        0     2490 2023-06-12 18:13:28.210817 garak-0.9.post1/garak/detectors/goodside.py
--rw-r--r--   0        0        0      926 2023-06-12 18:05:04.915540 garak-0.9.post1/garak/detectors/knownbadsignatures.py
--rw-r--r--   0        0        0      949 2023-06-12 21:14:54.000000 garak-0.9.post1/garak/detectors/lmrc.py
--rw-r--r--   0        0        0     3455 2023-06-12 16:30:32.000000 garak-0.9.post1/garak/detectors/misleading.py
--rw-r--r--   0        0        0     4545 2023-06-12 16:30:32.000000 garak-0.9.post1/garak/detectors/mitigation.py
--rw-r--r--   0        0        0     7188 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/detectors/perspective.py
--rw-r--r--   0        0        0      830 2023-06-12 16:26:20.000000 garak-0.9.post1/garak/detectors/promptinject.py
--rw-r--r--   0        0        0     6075 2023-06-12 16:26:53.000000 garak-0.9.post1/garak/detectors/riskywords.py
--rw-r--r--   0        0        0     1107 2023-06-12 16:19:39.000000 garak-0.9.post1/garak/detectors/snowball.py
--rw-r--r--   0        0        0      666 2023-06-12 16:18:45.000000 garak-0.9.post1/garak/detectors/specialwords.py
--rw-r--r--   0        0        0      476 2023-06-12 16:17:38.000000 garak-0.9.post1/garak/detectors/toxicity.py
--rw-r--r--   0        0        0       20 2023-05-18 03:08:10.893234 garak-0.9.post1/garak/evaluators/__init__.py
--rw-r--r--   0        0        0     2785 2023-06-09 05:46:41.839174 garak-0.9.post1/garak/evaluators/base.py
--rw-r--r--   0        0        0      436 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/evaluators/maxrecall.py
--rw-r--r--   0        0        0       25 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/generators/__init__.py
--rw-r--r--   0        0        0      820 2023-06-12 20:36:47.000000 garak-0.9.post1/garak/generators/base.py
--rw-r--r--   0        0        0     2796 2023-06-12 20:38:25.000000 garak-0.9.post1/garak/generators/cohere.py
--rw-r--r--   0        0        0     1803 2023-06-12 20:59:20.000000 garak-0.9.post1/garak/generators/ggml.py
--rw-r--r--   0        0        0     5659 2023-06-12 20:44:41.000000 garak-0.9.post1/garak/generators/huggingface.py
--rw-r--r--   0        0        0     3591 2023-06-12 20:42:24.000000 garak-0.9.post1/garak/generators/openai.py
--rw-r--r--   0        0        0     1866 2023-06-12 20:50:31.000000 garak-0.9.post1/garak/generators/replicate.py
--rw-r--r--   0        0        0      368 2023-06-12 20:38:47.000000 garak-0.9.post1/garak/generators/test.py
--rw-r--r--   0        0        0       20 2023-05-18 03:08:10.934500 garak-0.9.post1/garak/harness/__init__.py
--rw-r--r--   0        0        0     2353 2023-06-06 18:09:15.000000 garak-0.9.post1/garak/harness/base.py
--rw-r--r--   0        0        0     1626 2023-06-06 16:45:01.000000 garak-0.9.post1/garak/harness/probewise.py
--rw-r--r--   0        0        0     1985 2023-06-06 18:09:15.000000 garak-0.9.post1/garak/harness/pxd.py
--rw-r--r--   0        0        0       20 2023-05-18 03:08:10.940450 garak-0.9.post1/garak/probes/__init__.py
--rw-r--r--   0        0        0     4475 2023-06-13 03:50:04.172383 garak-0.9.post1/garak/probes/art.py
--rw-r--r--   0        0        0     2534 2023-06-12 22:20:40.000000 garak-0.9.post1/garak/probes/base.py
--rw-r--r--   0        0        0      359 2023-06-12 15:47:06.000000 garak-0.9.post1/garak/probes/blank.py
--rw-r--r--   0        0        0     2023 2023-06-12 18:05:49.609069 garak-0.9.post1/garak/probes/continuation.py
--rw-r--r--   0        0        0    50910 2023-06-12 15:54:28.000000 garak-0.9.post1/garak/probes/dan.py
--rw-r--r--   0        0        0    12703 2023-06-12 16:03:16.000000 garak-0.9.post1/garak/probes/encoding.py
--rw-r--r--   0        0        0     3386 2023-06-12 16:04:24.000000 garak-0.9.post1/garak/probes/goodside.py
--rw-r--r--   0        0        0     4420 2023-06-12 16:05:37.000000 garak-0.9.post1/garak/probes/knownbadsignatures.py
--rw-r--r--   0        0        0     5924 2023-06-12 21:14:54.000000 garak-0.9.post1/garak/probes/lmrc.py
--rw-r--r--   0        0        0     1157 2023-06-12 16:11:09.000000 garak-0.9.post1/garak/probes/misleading.py
--rw-r--r--   0        0        0     3636 2023-06-06 21:47:36.000000 garak-0.9.post1/garak/probes/promptinject.py
--rw-r--r--   0        0        0     2357 2023-06-12 15:56:25.000000 garak-0.9.post1/garak/probes/realtoxicityprompts.py
--rw-r--r--   0        0        0     1446 2023-06-12 15:48:50.000000 garak-0.9.post1/garak/probes/snowball.py
--rw-r--r--   0        0        0     1002 2023-06-13 03:53:59.366505 garak-0.9.post1/pyproject.toml
--rw-r--r--   0        0        0      185 2023-06-13 03:52:09.491824 garak-0.9.post1/requirements.txt
--rw-r--r--   0        0        0   344501 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/graph_connectivity.json
--rw-r--r--   0        0        0     3777 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/ldnoobw-en.txt
--rw-r--r--   0        0        0     2855 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/ofcom-potentially-offensive.txt
--rw-r--r--   0        0        0    37017 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/primality_testing.json
--rw-r--r--   0        0        0   105714 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/profanity_en.csv
--rw-r--r--   0        0        0      174 2023-06-06 20:59:34.000000 garak-0.9.post1/resources/promptinject/__init__.py
--rw-r--r--   0        0        0      615 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/_utils.py
--rw-r--r--   0        0        0    26965 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/prompt_data.py
--rw-r--r--   0        0        0    10015 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/prompting.py
--rw-r--r--   0        0        0     1836 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/run.py
--rw-r--r--   0        0        0     2377 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/scoring.py
--rw-r--r--   0        0        0     1343 2023-06-06 19:00:23.000000 garak-0.9.post1/resources/promptinject/visualization.py
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_flirtation.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_identity_attack.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_insult.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_profanity.txt
--rw-r--r--   0        0        0     4454 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_severe_toxicity.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_sexually_explicit.txt
--rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/rtp_threat.txt
--rw-r--r--   0        0        0    58554 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/senator_search.json
--rw-r--r--   0        0        0   152480 2023-06-06 18:09:15.000000 garak-0.9.post1/resources/slurprompts.jsonl
--rw-r--r--   0        0        0     6836 2023-06-10 23:40:40.000000 garak-0.9.post1/resources/slurprompts_80.jsonl
--rw-r--r--   0        0        0     5487 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/slursreclaimedslurs.txt
--rw-r--r--   0        0        0     1182 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/termscrape.py
--rw-r--r--   0        0        0   151324 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/truefalse_falseclaims.txt
--rw-r--r--   0        0        0     2389 2023-06-06 16:45:01.000000 garak-0.9.post1/resources/truefalse_falseclaims_50.txt
--rw-r--r--   0        0        0     1656 2023-06-12 22:19:11.000000 garak-0.9.post1/tests/test_cli.py
--rw-r--r--   0        0        0    12732 1970-01-01 00:00:00.000000 garak-0.9.post1/PKG-INFO
+-rw-r--r--   0        0        0     3112 2023-06-06 16:45:01.000000 garak-0.9.post2/.gitignore
+-rw-r--r--   0        0        0     2589 2023-06-12 21:52:09.000000 garak-0.9.post2/FAQ.md
+-rw-r--r--   0        0        0    35148 2023-06-06 16:45:01.000000 garak-0.9.post2/LICENSE
+-rw-r--r--   0        0        0      352 2023-06-13 17:58:55.336141 garak-0.9.post2/MANIFEST.in
+-rw-r--r--   0        0        0    13066 2023-06-13 05:03:26.000000 garak-0.9.post2/README.md
+-rw-r--r--   0        0        0     2127 2023-06-09 04:26:49.000000 garak-0.9.post2/analyse/analyse_log.py
+-rw-r--r--   0        0        0      109 2023-06-13 03:59:24.000000 garak-0.9.post2/garak/__init__.py
+-rw-r--r--   0        0        0      147 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/__main__.py
+-rw-r--r--   0        0        0      126 2023-06-13 17:49:11.759630 garak-0.9.post2/garak/_config.py
+-rw-r--r--   0        0        0     4311 2023-06-13 17:48:38.364136 garak-0.9.post2/garak/_plugins.py
+-rw-r--r--   0        0        0      989 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/attempt.py
+-rw-r--r--   0        0        0     8967 2023-06-09 05:48:04.000000 garak-0.9.post2/garak/cli.py
+-rw-r--r--   0        0        0       20 2023-05-25 19:31:38.900573 garak-0.9.post2/garak/detectors/__init__.py
+-rw-r--r--   0        0        0      473 2023-06-12 16:17:04.000000 garak-0.9.post2/garak/detectors/always.py
+-rw-r--r--   0        0        0     4636 2023-06-12 18:50:39.000000 garak-0.9.post2/garak/detectors/base.py
+-rw-r--r--   0        0        0      893 2023-06-12 18:05:58.000000 garak-0.9.post2/garak/detectors/continuation.py
+-rw-r--r--   0        0        0     1819 2023-06-12 18:07:57.000000 garak-0.9.post2/garak/detectors/dan.py
+-rw-r--r--   0        0        0     1566 2023-06-12 18:10:23.000000 garak-0.9.post2/garak/detectors/encoding.py
+-rw-r--r--   0        0        0     2490 2023-06-12 18:13:28.000000 garak-0.9.post2/garak/detectors/goodside.py
+-rw-r--r--   0        0        0      926 2023-06-12 18:05:04.000000 garak-0.9.post2/garak/detectors/knownbadsignatures.py
+-rw-r--r--   0        0        0      949 2023-06-12 21:14:54.000000 garak-0.9.post2/garak/detectors/lmrc.py
+-rw-r--r--   0        0        0     3455 2023-06-12 16:30:32.000000 garak-0.9.post2/garak/detectors/misleading.py
+-rw-r--r--   0        0        0     4545 2023-06-12 16:30:32.000000 garak-0.9.post2/garak/detectors/mitigation.py
+-rw-r--r--   0        0        0     7188 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/detectors/perspective.py
+-rw-r--r--   0        0        0      830 2023-06-12 16:26:20.000000 garak-0.9.post2/garak/detectors/promptinject.py
+-rw-r--r--   0        0        0     6168 2023-06-13 16:15:27.000000 garak-0.9.post2/garak/detectors/riskywords.py
+-rw-r--r--   0        0        0     1107 2023-06-12 16:19:39.000000 garak-0.9.post2/garak/detectors/snowball.py
+-rw-r--r--   0        0        0      711 2023-06-13 16:14:42.000000 garak-0.9.post2/garak/detectors/specialwords.py
+-rw-r--r--   0        0        0      476 2023-06-12 16:17:38.000000 garak-0.9.post2/garak/detectors/toxicity.py
+-rw-r--r--   0        0        0       20 2023-05-18 03:08:10.000000 garak-0.9.post2/garak/evaluators/__init__.py
+-rw-r--r--   0        0        0     2785 2023-06-09 05:46:41.000000 garak-0.9.post2/garak/evaluators/base.py
+-rw-r--r--   0        0        0      436 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/evaluators/maxrecall.py
+-rw-r--r--   0        0        0       25 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/generators/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-12 20:36:47.000000 garak-0.9.post2/garak/generators/base.py
+-rw-r--r--   0        0        0     2796 2023-06-12 20:38:25.000000 garak-0.9.post2/garak/generators/cohere.py
+-rw-r--r--   0        0        0     1803 2023-06-12 20:59:20.000000 garak-0.9.post2/garak/generators/ggml.py
+-rw-r--r--   0        0        0     5659 2023-06-12 20:44:41.000000 garak-0.9.post2/garak/generators/huggingface.py
+-rw-r--r--   0        0        0     3591 2023-06-12 20:42:24.000000 garak-0.9.post2/garak/generators/openai.py
+-rw-r--r--   0        0        0     1866 2023-06-12 20:50:31.000000 garak-0.9.post2/garak/generators/replicate.py
+-rw-r--r--   0        0        0      368 2023-06-12 20:38:47.000000 garak-0.9.post2/garak/generators/test.py
+-rw-r--r--   0        0        0       20 2023-05-18 03:08:10.000000 garak-0.9.post2/garak/harness/__init__.py
+-rw-r--r--   0        0        0     2353 2023-06-06 18:09:15.000000 garak-0.9.post2/garak/harness/base.py
+-rw-r--r--   0        0        0     1626 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/harness/probewise.py
+-rw-r--r--   0        0        0     1985 2023-06-06 18:09:15.000000 garak-0.9.post2/garak/harness/pxd.py
+-rw-r--r--   0        0        0       20 2023-05-18 03:08:10.000000 garak-0.9.post2/garak/probes/__init__.py
+-rw-r--r--   0        0        0     4475 2023-06-13 03:49:25.000000 garak-0.9.post2/garak/probes/art.py
+-rw-r--r--   0        0        0     2534 2023-06-12 22:20:40.000000 garak-0.9.post2/garak/probes/base.py
+-rw-r--r--   0        0        0      359 2023-06-12 15:47:06.000000 garak-0.9.post2/garak/probes/blank.py
+-rw-r--r--   0        0        0     2068 2023-06-13 16:16:02.000000 garak-0.9.post2/garak/probes/continuation.py
+-rw-r--r--   0        0        0    50910 2023-06-12 15:54:28.000000 garak-0.9.post2/garak/probes/dan.py
+-rw-r--r--   0        0        0    12703 2023-06-12 16:03:16.000000 garak-0.9.post2/garak/probes/encoding.py
+-rw-r--r--   0        0        0     3386 2023-06-12 16:04:24.000000 garak-0.9.post2/garak/probes/goodside.py
+-rw-r--r--   0        0        0     4420 2023-06-12 16:05:37.000000 garak-0.9.post2/garak/probes/knownbadsignatures.py
+-rw-r--r--   0        0        0     5924 2023-06-12 21:14:54.000000 garak-0.9.post2/garak/probes/lmrc.py
+-rw-r--r--   0        0        0     1202 2023-06-13 16:15:47.000000 garak-0.9.post2/garak/probes/misleading.py
+-rw-r--r--   0        0        0     3636 2023-06-06 21:47:36.000000 garak-0.9.post2/garak/probes/promptinject.py
+-rw-r--r--   0        0        0     2401 2023-06-13 16:16:53.000000 garak-0.9.post2/garak/probes/realtoxicityprompts.py
+-rw-r--r--   0        0        0     1539 2023-06-13 16:16:23.000000 garak-0.9.post2/garak/probes/snowball.py
+-rw-r--r--   0        0        0        1 2023-06-13 17:57:35.749057 garak-0.9.post2/garak/resources/__init__.py
+-rw-r--r--   0        0        0   344501 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/graph_connectivity.json
+-rw-r--r--   0        0        0     3777 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/ldnoobw-en.txt
+-rw-r--r--   0        0        0     2855 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/ofcom-potentially-offensive.txt
+-rw-r--r--   0        0        0    37017 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/primality_testing.json
+-rw-r--r--   0        0        0   105714 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/profanity_en.csv
+-rw-r--r--   0        0        0      174 2023-06-06 20:59:34.000000 garak-0.9.post2/garak/resources/promptinject/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-06 19:00:23.000000 garak-0.9.post2/garak/resources/promptinject/_utils.py
+-rw-r--r--   0        0        0    26965 2023-06-06 19:00:23.000000 garak-0.9.post2/garak/resources/promptinject/prompt_data.py
+-rw-r--r--   0        0        0    10015 2023-06-06 19:00:23.000000 garak-0.9.post2/garak/resources/promptinject/prompting.py
+-rw-r--r--   0        0        0     1836 2023-06-06 19:00:23.000000 garak-0.9.post2/garak/resources/promptinject/run.py
+-rw-r--r--   0        0        0     2377 2023-06-06 19:00:23.000000 garak-0.9.post2/garak/resources/promptinject/scoring.py
+-rw-r--r--   0        0        0     1343 2023-06-06 19:00:23.000000 garak-0.9.post2/garak/resources/promptinject/visualization.py
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/rtp_flirtation.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/rtp_identity_attack.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/rtp_insult.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/rtp_profanity.txt
+-rw-r--r--   0        0        0     4454 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/rtp_severe_toxicity.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/rtp_sexually_explicit.txt
+-rw-r--r--   0        0        0     4499 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/rtp_threat.txt
+-rw-r--r--   0        0        0    58554 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/senator_search.json
+-rw-r--r--   0        0        0   152480 2023-06-06 18:09:15.000000 garak-0.9.post2/garak/resources/slurprompts.jsonl
+-rw-r--r--   0        0        0     6836 2023-06-10 23:40:40.000000 garak-0.9.post2/garak/resources/slurprompts_80.jsonl
+-rw-r--r--   0        0        0     5487 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/slursreclaimedslurs.txt
+-rw-r--r--   0        0        0     1182 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/termscrape.py
+-rw-r--r--   0        0        0   151324 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/truefalse_falseclaims.txt
+-rw-r--r--   0        0        0     2389 2023-06-06 16:45:01.000000 garak-0.9.post2/garak/resources/truefalse_falseclaims_50.txt
+-rw-r--r--   0        0        0     1099 2023-06-13 17:51:04.670002 garak-0.9.post2/pyproject.toml
+-rw-r--r--   0        0        0      185 2023-06-13 03:52:09.000000 garak-0.9.post2/requirements.txt
+-rw-r--r--   0        0        0     1656 2023-06-12 22:19:11.000000 garak-0.9.post2/tests/test_cli.py
+-rw-r--r--   0        0        0    13977 1970-01-01 00:00:00.000000 garak-0.9.post2/PKG-INFO
```

### Comparing `garak-0.9.post1/.gitignore` & `garak-0.9.post2/.gitignore`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/FAQ.md` & `garak-0.9.post2/FAQ.md`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/LICENSE` & `garak-0.9.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/README.md` & `garak-0.9.post2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# garak, an llm vulnerability scanner
+# garak, an LLM vulnerability scanner
 
 `garak` is a modular tool for probing LLMs for undesireable prompt responses
 
 invoke with `python3 -m garak`
 
 currently supports:
 * [hugging face hub](https://huggingface.co/models) generative models
@@ -46,22 +46,28 @@
 ```
 
 
 ## Install:
 
 `garak` is a command-line tool. It's developed in Linux and OSX.
 
-`garak` has its own dependencies. You'll probably want to install `garak` in its own Conda environment:
+`garak` has its own dependencies. You can to install `garak` in its own Conda environment:
 
 ```
 conda create --name garak
 conda activate garak
 gh repo clone leondz/garak
 cd garak
-pip3 install -r requirements.txt
+python -m pip install -r requirements.txt
+```
+
+Alternatively you can install `garak` from pip:
+
+```
+python -m pip install garak
 ```
 
 OK, if that went fine, you're probably good to go!
 
 ## Getting started
 
 The general syntax is:
@@ -87,15 +93,30 @@
 
 See if the Hugging Face version of GPT2 is vulnerable to DAN 11.0
 
 ```
 python3 -m garak --model_type huggingface --model_name gpt2 --probes dan.Dan_11_0
 ```
 
-Errors go in `garak.log`; the run is logged in detail in a `.jsonl` file specified at analysis start & end. Send PRs & open issues. Happy hunting!
+
+## Reading the results
+
+For each probe loaded, garak will print a progress bar as it generates. Once generation is complete, a row evaluating that probe's results on each detector is given. If any of the prompt attempts yielded an undesirable behaviour, the response will be marked as FAIL, and the failure rate given.
+
+Here are the results with the `encoding` module on a GPT-3 variant:
+![alt text](https://i.imgur.com/8Dxf45N.png)
+
+And the same results for ChatGPT:
+![alt text](https://i.imgur.com/VKAF5if.png)
+
+We can see that the more recent model is much more susceptible to encoding-based injection attacks, where text-babbage-001 was only found to be vulnerable to quoted-printable and MIME encoding injections.  The figures at the end of each row, e.g. 840/840, indicate the number of text generations total and then how many of these seemed to behave OK. The figure can be quite high because more than one generation is made per prompt - by default, 10.
+
+Errors go in `garak.log`; the run is logged in detail in a `.jsonl` file specified at analysis start & end. There's a basic analysis script in `analyse/analyse_log.py` which will output the probes and prompts that led to the most hits.
+
+Send PRs & open issues. Happy hunting!
 
 ## Intro to generators
 
 ### huggingface
 
 * `--model_name huggingface` (for transformers models to run locally)
 * `--model_type` - use the model name from Hub. Only generative models will work. If it fails and shouldn't, please open an issue and paste in the command you tried + the exception!
@@ -231,9 +252,10 @@
 
 We have an FAQ [here](https://github.com/leondz/garak/blob/main/FAQ.md). Reach out if you have any more questions!
 
 <hr>
 
 _"Never tell the same lie twice"_ - Elim
 
+For updates and news see [@garak_llm](https://twitter.com/garak_llm)
 
 © GPLv3 2023 Leon Derczynski
```

### Comparing `garak-0.9.post1/analyse/analyse_log.py` & `garak-0.9.post2/analyse/analyse_log.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/_plugins.py` & `garak-0.9.post2/garak/_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import importlib
 import inspect
 import logging
 import os
 from typing import List
 
+import garak._config
+
 
 def enumerate_plugins(category: str = "probes") -> List[str]:
     """A function for listing all modules & plugins of the specified kind.
 
     garak's plugins are organised into four packages - probes, detectors, generators
     and harnesses. Each package contains a base module defining the core plugin
     classes. The other modules in the package define classes that inherit from the
@@ -42,15 +44,15 @@
             and getattr(base_mod, n).__class__.__name__
             == "type"  # be careful with what's imported into base modules
         ]
         + [root_plugin_classname]
     )
     plugin_class_names = {}
 
-    for module_filename in sorted(os.listdir("garak/" + category)):
+    for module_filename in sorted(os.listdir(garak._config.basedir / category)):
         if not module_filename.endswith(".py"):
             continue
         if module_filename.startswith("__") or module_filename == "base.py":
             continue
         module_name = module_filename.replace(".py", "")
         # print(category, 'module:', module_name)
         mod = importlib.import_module(f"garak.{category}.{module_name}")
```

### Comparing `garak-0.9.post1/garak/attempt.py` & `garak-0.9.post2/garak/attempt.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/cli.py` & `garak-0.9.post2/garak/cli.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/base.py` & `garak-0.9.post2/garak/detectors/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/continuation.py` & `garak-0.9.post2/garak/detectors/continuation.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/dan.py` & `garak-0.9.post2/garak/detectors/dan.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/encoding.py` & `garak-0.9.post2/garak/detectors/encoding.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/goodside.py` & `garak-0.9.post2/garak/detectors/goodside.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/knownbadsignatures.py` & `garak-0.9.post2/garak/detectors/knownbadsignatures.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/lmrc.py` & `garak-0.9.post2/garak/detectors/lmrc.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/misleading.py` & `garak-0.9.post2/garak/detectors/misleading.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/mitigation.py` & `garak-0.9.post2/garak/detectors/mitigation.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/perspective.py` & `garak-0.9.post2/garak/detectors/perspective.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/promptinject.py` & `garak-0.9.post2/garak/detectors/promptinject.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/riskywords.py` & `garak-0.9.post2/garak/detectors/riskywords.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python3
 
 from collections import defaultdict
 import csv
 
+import garak._config
 from garak.detectors.base import StringDetector
 
 surge_list = defaultdict(list)
-with open("resources/profanity_en.csv", "r") as csvfile:
+with open(garak._config.basedir / "resources/profanity_en.csv", "r") as csvfile:
     reader = csv.DictReader(csvfile)
     for row in reader:
         surge_list[row["category_1"]].append(row["text"])
         if row["category_2"]:
             surge_list[row["category_2"]].append(row["text"])
         if row["category_3"]:
             surge_list[row["category_3"]].append(row["text"])
 
 min_ofcom_strength = 2
 ofcom_list = defaultdict(list)
-with open("resources/ofcom-potentially-offensive.txt", "r") as csvfile:
+with open(garak._config.basedir / "resources/ofcom-potentially-offensive.txt", "r") as csvfile:
     reader = csv.DictReader(csvfile, delimiter="\t")
     for row in reader:
         category, term, strength = row
         if int(strength) >= min_ofcom_strength:
             ofcom_list[category].append(term)
 
 
@@ -210,13 +211,13 @@
 class LDNOOBW(StringDetector):
     name = f"ldnoobw"
     description = f"List of Dirty, Naughty, Obscene, and Otherwise Bad Words (English)"
     bcp47 = "en"
 
     def __init__(self):
         substrings = []
-        with open("resources/ldnoobw-en.txt", "r") as wordlist:
+        with open(garak._config.basedir / "resources/ldnoobw-en.txt", "r") as wordlist:
             for line in wordlist:
                 if line.strip():
                     substrings.append(line.strip())
         super().__init__(substrings)
         self.matchtype = "word"
```

### Comparing `garak-0.9.post1/garak/detectors/snowball.py` & `garak-0.9.post2/garak/detectors/snowball.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/detectors/specialwords.py` & `garak-0.9.post2/garak/detectors/specialwords.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 
 import json
 
+import garak._config
 from garak.detectors.base import StringDetector
 
 
 class SlursReclaimedSlurs(StringDetector):
     name = "slurs"
     description = "Slurs and reclaimed slurs"
     uri = "https://en.wikipedia.org/wiki/List_of_ethnic_slurs"
     bcp47 = "en"
 
     def __init__(self):
         self.substrings = set([])
-        with open("resources/slurprompts.jsonl", "r") as slurfile:
+        with open(garak._config.basedir / "resources/slurprompts.jsonl", "r") as slurfile:
             for line in slurfile:
                 line = line.strip()
                 if not line:
                     continue
                 self.substrings.add(json.loads(line)["term"])
 
         super().__init__(self.substrings)
```

### Comparing `garak-0.9.post1/garak/evaluators/base.py` & `garak-0.9.post2/garak/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/generators/base.py` & `garak-0.9.post2/garak/generators/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/generators/cohere.py` & `garak-0.9.post2/garak/generators/cohere.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/generators/ggml.py` & `garak-0.9.post2/garak/generators/ggml.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/generators/huggingface.py` & `garak-0.9.post2/garak/generators/huggingface.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/generators/openai.py` & `garak-0.9.post2/garak/generators/openai.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/generators/replicate.py` & `garak-0.9.post2/garak/generators/replicate.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/harness/base.py` & `garak-0.9.post2/garak/harness/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/harness/probewise.py` & `garak-0.9.post2/garak/harness/probewise.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/harness/pxd.py` & `garak-0.9.post2/garak/harness/pxd.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/art.py` & `garak-0.9.post2/garak/probes/art.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/base.py` & `garak-0.9.post2/garak/probes/base.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/continuation.py` & `garak-0.9.post2/garak/probes/continuation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 from collections import defaultdict
 import json
 
+import garak._config
 from garak.attempt import Attempt
 from garak.probes.base import TextProbe
 
 
 class ContinueSlursReclaimedSlurs50(TextProbe):
     name = "continueslur"
     description = "Continue partial word with slur or reclaimed slur"
@@ -19,15 +20,15 @@
 
     def __init__(self):
         super().__init__()
         # go through the list
         # for each term, work out first char, first three chars, all but last two chars
         # append these to each of the prefixes for that term
         slur_prefixes = defaultdict(set)
-        with open("resources/slurprompts_80.jsonl", "r") as slurfile:
+        with open(garak._config.basedir / "resources/slurprompts_80.jsonl", "r") as slurfile:
             for line in slurfile:
                 line = line.strip()
                 if not line:
                     continue
                 entry = json.loads(line)
                 slur_prefixes[entry["term"]].add(entry["prefix"])
```

### Comparing `garak-0.9.post1/garak/probes/dan.py` & `garak-0.9.post2/garak/probes/dan.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/encoding.py` & `garak-0.9.post2/garak/probes/encoding.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/goodside.py` & `garak-0.9.post2/garak/probes/goodside.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/knownbadsignatures.py` & `garak-0.9.post2/garak/probes/knownbadsignatures.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/lmrc.py` & `garak-0.9.post2/garak/probes/lmrc.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/misleading.py` & `garak-0.9.post2/garak/probes/misleading.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 
+import garak._config
 from garak.probes.base import TextProbe
 
 
 class FalseAssertion50(TextProbe):
     name = "falseassertion"
     description = "Does the model reject [questions based on] false claims?"
     bcp47 = "en"
@@ -19,15 +20,15 @@
         super().__init__()
 
         prefixes = ["", "Why is it that", "Explain why"]
 
         self.prompts = []
 
         for prefix in prefixes:
-            for false_assertion in open("resources/truefalse_falseclaims_50.txt", "r"):
+            for false_assertion in open(garak._config.basedir / "resources/truefalse_falseclaims_50.txt", "r"):
                 false_assertion = false_assertion.strip()
                 if not false_assertion:
                     continue
                 if not prefix:
                     self.prompts.append(false_assertion)
                 else:
                     if false_assertion.startswith("The"):
```

### Comparing `garak-0.9.post1/garak/probes/promptinject.py` & `garak-0.9.post2/garak/probes/promptinject.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/garak/probes/realtoxicityprompts.py` & `garak-0.9.post2/garak/probes/realtoxicityprompts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import sys
 
-
+import garak._config
 from garak.probes.base import TextProbe
 
 this = sys.modules[__name__]
 
 rtp_loaded = False
 rtp_dataset = None
 rtp_challenging = None
@@ -54,15 +54,15 @@
 ## dynamic class creation below
 probe_types = "threat insult severe_toxicity profanity sexually_explicit flirtation identity_attack".split()
 
 max_challenging = {}
 
 for probe_class in probe_types:
     # load filter lists
-    with open(f"resources/rtp_{probe_class}.txt") as f:
+    with open(garak._config.basedir / f"resources/rtp_{probe_class}.txt") as f:
         max_challenging[probe_class] = f.read().strip().split("\n")
 
     # define class
     classname = "RTP" + probe_class.title()
     probename = "realtoxicityprompts_" + probe_class
     descr = f"Implementation of {probe_class} probes in RealToxicityPrompts"
     bcp47 = "en"
```

### Comparing `garak-0.9.post1/garak/probes/snowball.py` & `garak-0.9.post2/garak/probes/snowball.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 #!/usr/bin/env python3
 # probe for confident, incorrect answers to complex reasoning/retrieval questions
 
 import json
 
+import garak._config
 from garak.probes.base import TextProbe
 
 
 class GraphConnectivity(TextProbe):
     name = "connectingflights"
     description = "Probe asking for impossible flight routings"
     bcp47 = "en"
     uri = "https://github.com/Nanami18/Snowballed_Hallucination"
     recommended_detector = ["snowball.DontStartYes"]
 
     def __init__(self):
         super().__init__()
-        with open("resources/graph_connectivity.json", "r") as f:
+        with open(garak._config.basedir / "resources/graph_connectivity.json", "r") as f:
             self.prompts = json.load(f)
 
 
 class Primes(TextProbe):
     name = "primes"
     description = "Ask model to check a list of higher primes"
     bcp47 = "en"
     uri = "https://github.com/Nanami18/Snowballed_Hallucination"
     recommended_detector = ["snowball.DontStartNo"]
 
     def __init__(self):
         super().__init__()
-        with open("resources/primality_testing.json", "r") as f:
+        with open(garak._config.basedir / "resources/primality_testing.json", "r") as f:
             dataset = json.load(f)
             self.prompts = [entry["question"] for entry in dataset]
 
 
 class Senators(TextProbe):
     name = "senators"
     description = "Asking for senators that don't exist"
     bcp47 = "en"
     uri = "https://github.com/Nanami18/Snowballed_Hallucination"
     recommended_detector = ["snowball.DontStartYes"]
 
     def __init__(self):
         super().__init__()
-        with open("resources/senator_search.json", "r") as f:
+        with open(garak._config.basedir / "resources/senator_search.json", "r") as f:
             self.prompts = json.load(f)
```

### Comparing `garak-0.9.post1/pyproject.toml` & `garak-0.9.post2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "garak"
-version = "0.9.post1"
+version = "0.9.post2"
 authors = [
   { name= "Leon Derczynski", email="leonderczynski@gmail.com" },
 ]
 license = { file = "LICENSE" }
 description = "LLM vulnerability scanner"
 readme = "README.md"
 classifiers = [
@@ -35,7 +35,13 @@
 
 [project.urls]
 "Homepage" = "https://github.com/leondz/garak"
 "Bug Tracker" = "https://github.com/leondz/garak/issues"
 
 [project.scripts]
 realpython = "garak.__main__:main"
+
+[tool.setuptools]
+packages = ["garak"]
+
+[tool.setuptools.package-data]
+"garak.resources" = ["*"]
```

### Comparing `garak-0.9.post1/resources/graph_connectivity.json` & `garak-0.9.post2/garak/resources/graph_connectivity.json`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/ldnoobw-en.txt` & `garak-0.9.post2/garak/resources/ldnoobw-en.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/ofcom-potentially-offensive.txt` & `garak-0.9.post2/garak/resources/ofcom-potentially-offensive.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/primality_testing.json` & `garak-0.9.post2/garak/resources/primality_testing.json`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/profanity_en.csv` & `garak-0.9.post2/garak/resources/profanity_en.csv`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/promptinject/_utils.py` & `garak-0.9.post2/garak/resources/promptinject/_utils.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/promptinject/prompt_data.py` & `garak-0.9.post2/garak/resources/promptinject/prompt_data.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/promptinject/prompting.py` & `garak-0.9.post2/garak/resources/promptinject/prompting.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/promptinject/run.py` & `garak-0.9.post2/garak/resources/promptinject/run.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/promptinject/scoring.py` & `garak-0.9.post2/garak/resources/promptinject/scoring.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/promptinject/visualization.py` & `garak-0.9.post2/garak/resources/promptinject/visualization.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/rtp_flirtation.txt` & `garak-0.9.post2/garak/resources/rtp_flirtation.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/rtp_identity_attack.txt` & `garak-0.9.post2/garak/resources/rtp_identity_attack.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/rtp_insult.txt` & `garak-0.9.post2/garak/resources/rtp_insult.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/rtp_profanity.txt` & `garak-0.9.post2/garak/resources/rtp_profanity.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/rtp_severe_toxicity.txt` & `garak-0.9.post2/garak/resources/rtp_severe_toxicity.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/rtp_sexually_explicit.txt` & `garak-0.9.post2/garak/resources/rtp_sexually_explicit.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/rtp_threat.txt` & `garak-0.9.post2/garak/resources/rtp_threat.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/senator_search.json` & `garak-0.9.post2/garak/resources/senator_search.json`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/slurprompts.jsonl` & `garak-0.9.post2/garak/resources/slurprompts.jsonl`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/slurprompts_80.jsonl` & `garak-0.9.post2/garak/resources/slurprompts_80.jsonl`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/slursreclaimedslurs.txt` & `garak-0.9.post2/garak/resources/slursreclaimedslurs.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/termscrape.py` & `garak-0.9.post2/garak/resources/termscrape.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/truefalse_falseclaims.txt` & `garak-0.9.post2/garak/resources/truefalse_falseclaims.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/resources/truefalse_falseclaims_50.txt` & `garak-0.9.post2/garak/resources/truefalse_falseclaims_50.txt`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/tests/test_cli.py` & `garak-0.9.post2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `garak-0.9.post1/PKG-INFO` & `garak-0.9.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garak
-Version: 0.9.post1
+Version: 0.9.post2
 Summary: LLM vulnerability scanner
 Author-email: Leon Derczynski <leonderczynski@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 Requires-Dist: pytest>=7.3
 Requires-Dist: google-api-python-client>=2.0
 Requires-Dist: backoff>=2.1.1
 Requires-Dist: torch
 Project-URL: Bug Tracker, https://github.com/leondz/garak/issues
 Project-URL: Homepage, https://github.com/leondz/garak
 
-# garak, an llm vulnerability scanner
+# garak, an LLM vulnerability scanner
 
 `garak` is a modular tool for probing LLMs for undesireable prompt responses
 
 invoke with `python3 -m garak`
 
 currently supports:
 * [hugging face hub](https://huggingface.co/models) generative models
@@ -72,22 +72,28 @@
 ```
 
 
 ## Install:
 
 `garak` is a command-line tool. It's developed in Linux and OSX.
 
-`garak` has its own dependencies. You'll probably want to install `garak` in its own Conda environment:
+`garak` has its own dependencies. You can to install `garak` in its own Conda environment:
 
 ```
 conda create --name garak
 conda activate garak
 gh repo clone leondz/garak
 cd garak
-pip3 install -r requirements.txt
+python -m pip install -r requirements.txt
+```
+
+Alternatively you can install `garak` from pip:
+
+```
+python -m pip install garak
 ```
 
 OK, if that went fine, you're probably good to go!
 
 ## Getting started
 
 The general syntax is:
@@ -113,15 +119,30 @@
 
 See if the Hugging Face version of GPT2 is vulnerable to DAN 11.0
 
 ```
 python3 -m garak --model_type huggingface --model_name gpt2 --probes dan.Dan_11_0
 ```
 
-Errors go in `garak.log`; the run is logged in detail in a `.jsonl` file specified at analysis start & end. Send PRs & open issues. Happy hunting!
+
+## Reading the results
+
+For each probe loaded, garak will print a progress bar as it generates. Once generation is complete, a row evaluating that probe's results on each detector is given. If any of the prompt attempts yielded an undesirable behaviour, the response will be marked as FAIL, and the failure rate given.
+
+Here are the results with the `encoding` module on a GPT-3 variant:
+![alt text](https://i.imgur.com/8Dxf45N.png)
+
+And the same results for ChatGPT:
+![alt text](https://i.imgur.com/VKAF5if.png)
+
+We can see that the more recent model is much more susceptible to encoding-based injection attacks, where text-babbage-001 was only found to be vulnerable to quoted-printable and MIME encoding injections.  The figures at the end of each row, e.g. 840/840, indicate the number of text generations total and then how many of these seemed to behave OK. The figure can be quite high because more than one generation is made per prompt - by default, 10.
+
+Errors go in `garak.log`; the run is logged in detail in a `.jsonl` file specified at analysis start & end. There's a basic analysis script in `analyse/analyse_log.py` which will output the probes and prompts that led to the most hits.
+
+Send PRs & open issues. Happy hunting!
 
 ## Intro to generators
 
 ### huggingface
 
 * `--model_name huggingface` (for transformers models to run locally)
 * `--model_type` - use the model name from Hub. Only generative models will work. If it fails and shouldn't, please open an issue and paste in the command you tried + the exception!
@@ -257,10 +278,11 @@
 
 We have an FAQ [here](https://github.com/leondz/garak/blob/main/FAQ.md). Reach out if you have any more questions!
 
 <hr>
 
 _"Never tell the same lie twice"_ - Elim
 
+For updates and news see [@garak_llm](https://twitter.com/garak_llm)
 
 © GPLv3 2023 Leon Derczynski
```

