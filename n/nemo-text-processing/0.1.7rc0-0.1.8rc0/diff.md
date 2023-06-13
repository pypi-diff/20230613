# Comparing `tmp/nemo_text_processing-0.1.7rc0.tar.gz` & `tmp/nemo_text_processing-0.1.8rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_text_processing-0.1.7rc0.tar", last modified: Thu Mar  9 23:09:29 2023, max compression
+gzip compressed data, was "nemo_text_processing-0.1.8rc0.tar", last modified: Tue Jun 13 19:48:46 2023, max compression
```

## Comparing `nemo_text_processing-0.1.7rc0.tar` & `nemo_text_processing-0.1.8rc0.tar`

### file list

```diff
@@ -1,1252 +1,1371 @@
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.019338 nemo_text_processing-0.1.7rc0/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11356 2022-11-08 00:24:38.000000 nemo_text_processing-0.1.7rc0/LICENSE
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2022-11-29 20:12:30.000000 nemo_text_processing-0.1.7rc0/MANIFEST.in
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5718 2023-03-09 23:09:29.019338 nemo_text_processing-0.1.7rc0/PKG-INFO
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4204 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/README.md
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.871339 nemo_text_processing-0.1.7rc0/nemo_text_processing/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.871339 nemo_text_processing-0.1.7rc0/nemo_text_processing/fst_alignment/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      622 2022-12-16 17:13:41.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/fst_alignment/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9241 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/fst_alignment/alignment.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.871339 nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      622 2022-12-16 17:13:41.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3439 2022-12-16 17:13:41.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/mlm_scorer.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6235 2022-12-16 17:13:41.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/model_utils.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    26836 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/utils.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12854 2022-12-16 17:13:41.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/wfst_lm_rescoring.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.871339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      707 2022-12-16 17:13:41.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.871339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      997 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.875339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      997 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1579 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2471 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4812 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3325 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1188 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4718 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1210 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1240 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.875339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      966 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1667 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2359 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2055 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2914 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1829 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1749 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1295 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.875339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      923 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.879339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3298 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3578 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2643 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1594 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2658 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3901 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3571 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1628 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2077 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1981 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8456 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1700 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.879339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1475 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1977 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2440 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1523 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2470 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2446 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1815 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.879339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      923 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12771 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.883339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3146 2023-01-30 23:48:40.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      137 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/date_period.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.883339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       32 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      121 2023-02-13 14:02:25.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      263 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       42 2023-01-30 23:48:40.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/url_symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       41 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/magnitudes.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2183 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/months.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/months_cased.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.883339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       62 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/hundred.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      109 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      261 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/thousands.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       78 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.883339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/teen.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.883339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/minute_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-02-15 06:23:58.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix_cased.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-02-15 06:24:02.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone_cased.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       89 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/to_hour.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5481 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/year_suffix.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.887339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9965 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7650 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5152 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5519 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1098 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4358 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5174 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2067 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1218 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8702 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6893 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5776 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2187 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1240 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1620 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.887339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1655 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3033 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2346 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1883 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      916 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2192 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1483 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2042 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1550 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2696 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2867 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1779 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1382 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1325 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.887339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      936 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.887339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.891339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       88 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/months.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      253 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/year_suffix.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.891339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      117 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      311 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/symbols.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.891339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       85 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/numbers_read_as_ordinals.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       28 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/ordinal_exceptions.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.891339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       29 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/math_symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      439 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      432 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_singular.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.891339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      739 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4273 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      660 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3933 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       73 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      743 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       68 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      807 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       88 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/months.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.891339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       77 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      239 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      108 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       82 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      158 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/twenties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.895339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      280 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      473 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1324 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      312 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1403 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.895339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       15 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/thousands.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/ties.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.895339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       95 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/minutes_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      157 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      448 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1056 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3192 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      219 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/whitelist.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1988 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.895339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8079 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3382 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4964 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4011 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4980 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5579 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5539 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4369 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1189 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5702 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7799 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5776 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1808 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1211 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      864 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.899339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1668 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2386 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2901 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1973 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1893 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2558 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1484 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1644 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1246 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2711 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3057 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1750 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1353 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1296 2022-12-15 01:23:43.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.899339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      936 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.899339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.899339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       77 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      120 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      126 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      737 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.899339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      122 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/magnitudes.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      391 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/measurements.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.899339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      674 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       60 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_minor.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       87 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/months.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.899339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       68 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       10 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       57 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      236 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/thousands.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      146 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      470 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties_unique.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        8 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.903339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      318 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/digits_root_change.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       51 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/firsts.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/key_nouns.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       43 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/second.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.903339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/digits_large.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/hundreds_large.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/ties_large.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        0 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/suppletive.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.903339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/hour_to_night.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      255 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/hours.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/hours_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      881 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      353 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        8 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_am.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_pm.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      300 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/whitelist.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6039 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.903339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11883 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2600 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5181 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4382 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3342 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3387 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5784 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3458 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1292 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4480 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5584 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5822 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1795 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1219 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      864 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.907339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1676 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2543 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3587 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1660 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1943 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2566 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1514 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3202 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1258 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2326 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3060 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1758 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1382 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1325 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8709 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/inverse_normalize.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.907339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      936 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.907339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       74 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/currency_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       65 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/currency_singular.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.907339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       80 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       80 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      890 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      814 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       90 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/months.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.907339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       77 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      213 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/onehundred.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      113 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       80 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      128 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/twenties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.911339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      167 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      471 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      281 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/ties.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.911339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        3 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_am.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        4 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_pm.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      119 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/hours_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      353 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/minutes_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       45 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_am.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       35 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_pm.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/whitelist.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.911339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    16257 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3500 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5042 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4010 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3536 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5062 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3608 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1189 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4999 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9384 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5498 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1808 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1211 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      856 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.915339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1668 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2775 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2901 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1973 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2163 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1513 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1568 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1245 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2625 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2839 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1749 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1369 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1296 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.915339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.915339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1873 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1536 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2575 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1575 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1600 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1513 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1695 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1705 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2984 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6004 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1877 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.915339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1770 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1194 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1929 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1216 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1346 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1211 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1452 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1232 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1778 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2817 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1750 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4898 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/run_evaluate.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.915339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      923 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.919339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/currency.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.919339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       35 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      113 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      213 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       40 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/magnitudes.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.919339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       82 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2692 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      120 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/months.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.919339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       71 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        5 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/hundred.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      172 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       54 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/thousands.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       63 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        8 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.919339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       85 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/digit.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.919339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      356 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to_night.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1789 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      335 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/time_suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/time_zone.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        0 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/whitelist.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5045 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.923339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6393 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6159 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5055 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3718 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2386 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3654 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2819 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1512 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1223 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1774 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4463 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5849 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1845 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1246 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      843 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.923339 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1659 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2734 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2340 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1885 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1761 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2689 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1489 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1397 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1276 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3037 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3071 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1786 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1409 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1352 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1445 2023-03-09 23:01:22.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/package_info.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.927339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      777 2022-12-16 17:13:41.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.927339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1228 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.927339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.927339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      577 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       57 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/currency_minor_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       30 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/currency_minor_singular.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      552 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.931339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      107 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/digit_100.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       83 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/digit_1000.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      432 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/flops.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/fraction.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      118 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/fraction_dual.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/fraction_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       82 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/fraction_singular.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       73 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/quantities.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      175 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/teens.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/tens.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       10 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/zero.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8531 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.931339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      966 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4554 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3367 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8424 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5119 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1324 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1656 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.931339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      966 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1783 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2248 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4514 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3118 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2133 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2877 2023-02-10 23:20:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1525 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12054 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/data_loader_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.935339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.935339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.935339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      118 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       84 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      258 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/electronic/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      542 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/fractions.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.935339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/measure/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/measure/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1198 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      139 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/measure/suppletive.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.935339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      396 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/money/currency.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/money/currency_minor_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/money/currency_minor_singular.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.935339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/months/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/months/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      147 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/months/abbr_to_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      230 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/months/numbers.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.939339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       59 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/ones.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      119 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/quantities.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      109 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       81 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.939339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       93 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/ordinals/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       70 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/ordinals/thousands.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      139 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/ordinals/ties.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.939339 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       53 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/time/hour_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/time/hour_to_night.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/time/minute_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/time/time_zone.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       89 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/whitelist.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.943338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7655 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5769 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3691 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3196 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2225 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7045 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7225 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2001 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3700 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3980 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7240 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2810 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1312 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1300 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.943338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1733 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2758 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2434 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3560 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3029 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2128 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3377 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2302 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1849 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5517 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3770 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2877 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.943338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      899 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12763 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/clean_eval_data.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.943338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.943338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/address/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/address/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      161 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/address/address_word.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      617 2023-01-04 21:13:00.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/address/state.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.947338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      257 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/day.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      141 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/month_abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/month_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      234 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/month_number.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      128 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/year_suffix.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.947338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-02-01 05:36:22.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      222 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/electronic/symbol.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/electronic/words.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.947338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       71 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/math_operation.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1554 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/unit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      544 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.947338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      656 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       36 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/currency_minor_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/currency_minor_singular.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       15 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/per_unit.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.947338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)   325078 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    54511 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       62 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/fraction.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/hundred.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      107 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/quantity_abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      109 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      261 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/thousand.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       69 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/ty.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.951338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/ordinal/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/ordinal/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/ordinal/teen.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.951338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    35561 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/female.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       45 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/key_word.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    20334 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/male.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    72815 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1843 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/suppletive.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.951338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/telephone/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/telephone/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       19 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/telephone/ip_prompt.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       38 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/telephone/ssn_prompt.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       56 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/telephone/telephone_prompt.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.951338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       84 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/time/suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      116 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/time/zone.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.951338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      520 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      155 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives_all_format.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)   175146 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      865 2023-01-11 17:04:50.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2532 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      263 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/lj_speech.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      240 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/symbol.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    36553 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9092 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.955338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2069 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/abbreviation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7173 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    15335 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5489 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4911 2023-02-15 05:08:57.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2400 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11524 2023-01-18 18:57:07.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9521 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2548 2023-02-16 18:24:35.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2565 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4936 2023-01-23 22:53:50.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/range.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4551 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/roman.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6174 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/serial.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6034 2023-02-15 05:09:08.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5199 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10997 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12339 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12789 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6289 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3999 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1643 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.955338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1446 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1953 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3925 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3294 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4599 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3719 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4473 2023-01-23 22:53:50.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2742 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2112 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6806 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2508 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/roman.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2372 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3637 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3986 2023-01-31 19:29:33.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3163 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1581 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1511 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.959338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      682 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.959338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.959338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      348 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/days_abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      115 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/months.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      551 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1184 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.959338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       73 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      311 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/electronic/symbols.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.959338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/fractions/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/fractions/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      117 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/fractions/fraction_symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       28 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/fractions/ordinal_exceptions.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      224 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      137 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten_fem.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.959338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/math_symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      260 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/measurements.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       95 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_complex.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       55 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_fem.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      537 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.959338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1030 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4219 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      773 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2155 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      177 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1800 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1277 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5659 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.963338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      111 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/quantities.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      108 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       72 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      141 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/twenties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.963338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      137 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      286 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/gender_suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      471 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      200 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      165 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      295 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/twenties.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.963338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/roman/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/roman/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/roman/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/roman/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       15 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/roman/thousands.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/roman/ties.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.963338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/telephone/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/telephone/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       66 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/telephone/ip_prompt.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      143 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/telephone/telephone_prompt.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.963338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       31 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/afternoon_times.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/alt_minutes.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/evening_times.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       53 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/hour_to_12.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      128 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/hour_to_24.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/hour_to_night.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/minute_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       60 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/morning_times.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      150 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/time_suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1056 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3192 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      869 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/whitelist.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8364 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.967338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7734 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5597 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6087 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/decimals.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3463 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5930 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10331 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8829 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7371 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8012 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9640 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7341 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2810 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1326 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1140 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.967338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2398 2023-01-24 00:18:17.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3468 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3706 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/decimals.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3586 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8534 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6198 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7013 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2961 2023-01-24 00:18:13.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2517 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8939 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3589 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2873 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    30715 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/normalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    22441 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/normalize_with_audio.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2891 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/preprocessing_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.967338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2077 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/alphabet.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.971338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.971338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/currency/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/currency/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1420 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1085 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.971338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       47 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      290 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      668 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      275 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/latin_to_cyrillic.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9277 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/measurements.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.971338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/months/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/months/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      239 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/months/abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1541 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      214 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/months/numbers.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.971338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      969 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      911 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      933 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      913 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1048 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      951 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      549 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      710 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      565 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1026 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      119 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/digits_nominative_case.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      430 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/ordinal_endings.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    21537 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      537 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.971338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      469 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_cardinal.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      611 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      828 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       62 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/time_convert.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.979338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3206 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/g.fst
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    69495 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)  7085564 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    14099 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1005 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/whitelist.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.983338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6818 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6014 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4465 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/decimals.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4796 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6942 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3997 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6605 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/number_names.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2950 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3265 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5253 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7139 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3044 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1312 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1287 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.983338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1891 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1497 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2189 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1570 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1759 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1494 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1462 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1782 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2115 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2993 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2925 2022-12-15 01:23:44.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5055 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/run_evaluate.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.983338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.983338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      334 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/abbreviations_nondet.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.987338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/dates/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/dates/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      116 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/dates/era_suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       94 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/dates/era_words.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      176 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/dates/month_abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      112 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/dates/months.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.987338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/electronic/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/electronic/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/electronic/domain.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      289 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/electronic/server_name.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      263 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/electronic/symbols.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       71 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/math_operations.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.987338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      196 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/greek_lower.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      196 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/greek_upper.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2121 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      157 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/unit_neuter.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1461 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.987338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1344 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_major_nt.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      745 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      735 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1197 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.987338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       57 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/fraction.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1586 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/millions_abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      330 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/quantities.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       94 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       72 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.987338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/ordinals/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/ordinals/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       83 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/ordinals/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      115 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/ordinals/teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       96 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/ordinals/ties.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        9 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/ordinals/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.991338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/roman/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/roman/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/roman/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/roman/hundreds.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/roman/ties.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.991338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       22 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/ip_prompt.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       96 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/special_numbers.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       28 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/ssn_prompt.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      381 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/telephone_abbr.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       58 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/telephone_prompt.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.991338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       53 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/hour_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/hour_to_night.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/minute_to.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      261 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/time_zone.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1046 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/whitelist.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2520 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.991338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2167 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    17281 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7019 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6753 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3466 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4169 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10130 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12279 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9421 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6677 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8756 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9256 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11099 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3023 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1322 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1181 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1732 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2631 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2837 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3678 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3155 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3753 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2806 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1584 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2743 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4270 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3589 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2873 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5164 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/token_parser.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10972 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/utils_audio_based.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/charset_extension.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    32616 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      553 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       13 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/oov_tags.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      288 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/punctuations_zh.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       72 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/upper_to_lower.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/date/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/date/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/date/year_suffix.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/denylist/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/denylist/denylist.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/erhua/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      350 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/erhua/whitelist.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/math/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/math/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/math/score.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/math/symbol.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.995338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/measure/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/measure/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1138 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      988 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/measure/units_zh.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.999338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/money/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/money/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2374 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/money/currency_code.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1311 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/money/currency_symbol.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.999338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/number/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/number/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       54 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/number/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       51 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/number/digit_teen.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       12 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/number/sign.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/number/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.999338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       19 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/digit.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       63 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/hour.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      108 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/suffix.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/tens.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        2 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/zero.tsv
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.999338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/whitelist/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/whitelist/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      687 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/whitelist/default.tsv
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4023 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/graph_utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.999338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5168 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1087 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/char.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4010 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1491 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1652 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/math_symbol.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2079 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1789 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1850 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2678 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4535 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1611 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1728 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.003338 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1190 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1100 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/char.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2847 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1458 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1139 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/math_symbol.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1885 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1379 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3046 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3481 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2813 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2222 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1289 2022-11-14 19:50:21.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:28.871339 nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5718 2023-03-09 23:09:28.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/PKG-INFO
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    73040 2023-03-09 23:09:28.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/SOURCES.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        1 2023-03-09 23:09:28.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/dependency_links.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        1 2022-12-13 23:20:30.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/not-zip-safe
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      465 2023-03-09 23:09:28.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/requires.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-03-09 23:09:28.000000 nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/top_level.txt
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.003338 nemo_text_processing-0.1.7rc0/requirements/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      138 2023-03-09 23:00:43.000000 nemo_text_processing-0.1.7rc0/requirements/requirements.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      158 2023-02-09 20:01:15.000000 nemo_text_processing-0.1.7rc0/requirements/requirements_test.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1142 2023-03-09 23:09:29.019338 nemo_text_processing-0.1.7rc0/setup.cfg
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8341 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/setup.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.003338 nemo_text_processing-0.1.7rc0/tests/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8115 2022-11-15 05:09:39.000000 nemo_text_processing-0.1.7rc0/tests/conftest.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.003338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.003338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2326 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2313 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2322 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2331 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2326 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2323 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2317 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1546 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_normalization_with_audio.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2046 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2329 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2313 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2329 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2314 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.007338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1885 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_address.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3053 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3752 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2950 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2943 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1785 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1842 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_math.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2931 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3030 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1530 2023-02-01 02:09:00.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_normalization_with_audio.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2942 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1839 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_punctuation.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1847 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_range.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1852 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_roman.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1865 2023-01-23 22:53:50.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_serial.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1956 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_special_text.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2962 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1748 2022-12-14 17:06:16.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_text_split.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2928 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3635 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3024 2023-03-08 02:31:46.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.007338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2338 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2258 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2334 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2352 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1809 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2344 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2329 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1507 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_normalization_with_audio.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2335 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2349 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2334 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2347 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2396 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.011338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1282 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1279 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1285 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1282 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1276 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1274 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.011338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1282 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1279 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1285 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1276 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1274 2023-01-26 19:24:54.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.011338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.011338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      972 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_cardinal.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1712 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_cardinal_normalize_with_audio.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      458 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_date.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1003 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_decimal.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      527 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_electronic.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      788 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_measure.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      567 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_money.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2913 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_ordinal.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      166 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_telephone.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      415 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_time.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       87 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_whitelist.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      215 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/test_cases_word.txt
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6340 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6527 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/test_ru_normalization.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.015338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/__init__.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.015338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/data_text_normalization/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-01-30 22:12:32.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/data_text_normalization/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1793 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1786 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1791 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1797 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1794 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1792 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1788 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1602 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_normalization_with_audio.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1793 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1796 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1786 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1795 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1834 2023-03-09 23:00:13.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_word.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2251 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/utils.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.015338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1600 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_cardinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1591 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1597 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_decimal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1603 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_electronic.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1600 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1598 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1594 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1598 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_ordinal.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1602 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_telephone.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1591 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_time.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1602 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_whitelist.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1592 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_word.py
-drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-03-09 23:09:29.015338 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/__init__.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1257 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_char.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1244 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_date.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1269 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_fraction.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1257 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_math.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1266 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_measure.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1230 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_money.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1275 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_preprocess.py
--rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1257 2022-11-14 22:54:30.000000 nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_time.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.155345 nemo_text_processing-0.1.8rc0/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11356 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/LICENSE
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/MANIFEST.in
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5718 2023-06-13 19:48:46.155345 nemo_text_processing-0.1.8rc0/PKG-INFO
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4204 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/README.md
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/fst_alignment/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      622 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/fst_alignment/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9241 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/fst_alignment/alignment.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/g2p/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-06-08 22:44:38.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/g2p/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/g2p/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-06-08 22:44:38.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/g2p/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      622 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3439 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/mlm_scorer.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6235 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/model_utils.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    26836 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/utils.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12854 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/wfst_lm_rescoring.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      707 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      997 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      997 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1579 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2505 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4812 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2985 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3325 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1188 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5125 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1210 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1240 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      966 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1667 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2359 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2055 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2223 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2914 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2060 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1749 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1295 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      923 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.011347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3298 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3578 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2643 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1594 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2658 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3901 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3571 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1628 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2077 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1981 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8456 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1700 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.011347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1475 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1977 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2440 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1523 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2470 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2446 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1815 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.011347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      923 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12771 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.011347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3146 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      137 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/date_period.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.011347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       32 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      121 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      263 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       42 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/url_symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       41 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/magnitudes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2183 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/months.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/months_cased.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.015347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       62 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/hundred.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      109 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      261 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/thousands.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       78 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.015347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/teen.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.015347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/minute_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_suffix_cased.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/time_zone_cased.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       89 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/to_hour.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5481 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/year_suffix.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.015347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9965 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7648 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5152 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5519 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1098 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4358 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5174 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2067 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1218 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8702 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6893 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5776 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2187 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1240 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1620 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.019347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1655 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3031 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2346 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1883 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      916 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2192 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1483 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2042 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1550 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2696 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2867 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1779 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1382 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1325 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.019347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      936 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.019347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.019347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       88 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/months.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      253 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/year_suffix.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.019347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      117 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      311 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/symbols.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.019347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       85 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/numbers_read_as_ordinals.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       28 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/ordinal_exceptions.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.019347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       29 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/math_symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      439 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      432 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/measurements_singular.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.023347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      739 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4273 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      660 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3933 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      743 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       58 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      807 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       88 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/months.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.023347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       77 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      239 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      108 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       82 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      158 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/twenties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.023347 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      280 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      473 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1324 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      312 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1403 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.027346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       15 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/thousands.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/ties.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.027346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       95 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/minutes_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      157 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      448 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1056 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3192 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      219 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/whitelist.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1988 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.027346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8079 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3382 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4964 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4011 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4980 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5579 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5539 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4369 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1189 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5702 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7799 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5776 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1808 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1211 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      864 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.027346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1668 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2386 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2901 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1973 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1893 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2558 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1484 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1644 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1246 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2711 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3057 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1750 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1353 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1296 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.027346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      936 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.027346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.031346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       77 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      120 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      126 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      737 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.031346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      122 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/magnitudes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      391 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/measurements.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.031346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      674 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       60 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_minor.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       87 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/months.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.031346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       68 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       10 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       57 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      236 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/thousands.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      146 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      470 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/ties_unique.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        8 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.031346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      318 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/digits_root_change.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       51 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/firsts.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/key_nouns.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       43 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/second.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.031346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/digits_large.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/hundreds_large.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/ties_large.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/suppletive.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.035346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/hour_to_night.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      255 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/hours.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/hours_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      881 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      353 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        8 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_am.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/time_suffix_pm.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      300 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/whitelist.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6051 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.035346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11883 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2600 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5181 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4382 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3342 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3387 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5784 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3458 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1292 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4480 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5584 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5822 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1795 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1219 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      864 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.035346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1676 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2543 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3587 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1660 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1943 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2566 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1514 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3202 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1258 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2326 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3060 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1758 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1382 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1325 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8709 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/inverse_normalize.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.035346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      936 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.039346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       74 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/currency_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       65 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/currency_singular.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.039346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       80 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       80 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/symbols.tsv
+-rwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)      890 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv
+-rwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)      814 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       90 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/months.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.039346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       77 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      213 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/onehundred.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      113 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       80 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      128 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/twenties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.039346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      167 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      471 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      281 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/ties.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.039346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        3 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_am.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        4 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/hour_to_pm.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      119 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/hours_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      353 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/minutes_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       45 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_am.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       35 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/time_suffix_pm.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/whitelist.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.043346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    16257 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3500 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5042 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4010 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3536 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5062 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3608 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1189 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py
+-rwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)     4999 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py
+-rwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)     9384 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5498 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1808 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1211 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      856 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.043346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1668 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2775 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2901 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1973 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2163 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1513 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1568 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1245 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py
+-rwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)     2625 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2839 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1749 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1369 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1296 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.043346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.043346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1873 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1536 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2575 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1575 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1600 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1513 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1695 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1705 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2984 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6004 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1877 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.043346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1770 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1194 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1929 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1216 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1346 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1211 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1452 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1232 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1778 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2817 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1750 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4898 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/run_evaluate.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.043346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      923 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.047346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/currency.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.047346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       35 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      113 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      213 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       40 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/magnitudes.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.047346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       82 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2692 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      120 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/months.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.047346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       71 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        5 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/hundred.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      172 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       54 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/thousands.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       63 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        8 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.047346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       85 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/digit.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.051346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      356 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/hours_to_night.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1789 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      335 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       61 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/time_suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/time_zone.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/whitelist.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5067 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.051346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6393 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6159 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5055 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3718 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2386 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3654 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2819 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1512 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1223 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1774 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4463 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5849 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1845 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1246 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      843 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.051346 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1659 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2734 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2340 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1885 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1761 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2689 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1489 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1397 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1276 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3037 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3071 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1786 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1409 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1352 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1445 2023-06-13 19:47:30.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/package_info.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.051346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      777 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.051346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1228 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.051346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.051346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/measure/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/measure/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      317 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/measure/measurements.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.055346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      577 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       57 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/currency_minor_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       30 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/currency_minor_singular.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      552 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.055346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      107 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/digit_100.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       83 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/digit_1000.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      432 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/flops.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/fraction.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      118 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/fraction_dual.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/fraction_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       82 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/fraction_singular.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       73 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/quantities.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      175 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/teens.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/tens.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       10 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/zero.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8553 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.055346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      966 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4554 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3367 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6003 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8424 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5470 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1324 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1656 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      966 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1783 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2248 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4514 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2123 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3118 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2384 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2877 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1525 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12054 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/data_loader_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      118 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       84 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      258 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/electronic/symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      542 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/fractions.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/measure/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/measure/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1198 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      139 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/measure/suppletive.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      396 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/money/currency.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/money/currency_minor_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/money/currency_minor_singular.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/months/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/months/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      147 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/months/abbr_to_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      230 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/months/numbers.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.059346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       59 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/ones.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      119 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/quantities.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      109 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       81 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.063346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       93 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/ordinals/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       70 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/ordinals/thousands.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      139 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/ordinals/ties.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.063346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       53 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/time/hour_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/time/hour_to_night.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/time/minute_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/time/time_zone.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       89 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/whitelist.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.063346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7655 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5769 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3691 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3196 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2225 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7045 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7225 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2001 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3700 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3980 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7240 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2810 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1312 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1300 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.063346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1733 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2758 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2434 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3560 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3029 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2128 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3377 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2302 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1849 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5517 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3770 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2877 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.063346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      899 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12763 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/clean_eval_data.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.063346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.063346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/address/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/address/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      161 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/address/address_word.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      617 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/address/state.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.067346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      257 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/day.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      141 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/month_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/month_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      234 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/month_number.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      128 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/year_suffix.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.067346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      222 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/electronic/symbol.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      129 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/electronic/words.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.067346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       71 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/math_operation.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1554 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/unit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      544 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.067346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      656 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       36 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/currency_minor_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/currency_minor_singular.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       15 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/per_unit.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.071346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/__init__.py
+-rwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)   325078 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    54511 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       62 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/fraction.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/hundred.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      107 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/quantity_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      109 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      261 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/thousand.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       69 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/ty.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.071346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/ordinal/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/ordinal/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/ordinal/teen.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.071346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    35561 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/female.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       45 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/key_word.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    20334 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/male.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    72815 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1843 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/suppletive.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.071346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/telephone/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/telephone/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       19 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/telephone/ip_prompt.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       38 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/telephone/ssn_prompt.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       56 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/telephone/telephone_prompt.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.071346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       84 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/time/suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      116 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/time/zone.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.075346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      520 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      155 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives_all_format.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)   175146 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      865 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2532 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      263 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/lj_speech.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      240 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/symbol.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    36553 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9122 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.075346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2069 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/abbreviation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7173 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    15333 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5489 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5056 2023-06-13 19:46:44.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2400 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11524 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9521 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2548 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2565 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/punctuation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4936 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/range.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4551 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/roman.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6174 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/serial.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6034 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5199 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10997 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12339 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12789 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6289 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3999 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1643 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.075346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1446 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1953 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3923 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3294 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4599 2023-06-06 21:28:53.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3719 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4473 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2742 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2112 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6806 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2508 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/roman.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2372 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3637 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3986 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3163 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1581 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1511 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.075346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      682 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.079346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.079346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      348 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/days_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      115 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/months.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      551 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1184 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.079346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       86 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       73 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      311 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/electronic/symbols.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.079346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/fractions/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/fractions/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      117 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/fractions/fraction_symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       28 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/fractions/ordinal_exceptions.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      224 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      137 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/fractions/powers_of_ten_fem.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.079346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/math_symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      260 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/measurements.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       95 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_complex.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       55 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_fem.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      537 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.083346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1030 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4219 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      773 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2155 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      177 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1800 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1277 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5659 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.083346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      111 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/quantities.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      108 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       72 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      141 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/twenties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.083346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      137 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      286 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/gender_suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      471 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      200 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      165 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      295 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/twenties.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.087346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/roman/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/roman/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/roman/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/roman/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       15 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/roman/thousands.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/roman/ties.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.087346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/telephone/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/telephone/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       66 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/telephone/ip_prompt.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      143 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/telephone/telephone_prompt.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.087346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       31 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/afternoon_times.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/alt_minutes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/evening_times.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       53 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/hour_to_12.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      128 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/hour_to_24.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/hour_to_night.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/minute_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       60 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/morning_times.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      150 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/time_suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1056 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3192 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      869 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/whitelist.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8364 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.087346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7734 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5597 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6239 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/decimals.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3463 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5930 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7949 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8829 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7371 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8012 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9439 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7342 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2810 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1326 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1140 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.087346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2398 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3468 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3706 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/decimals.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3586 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8534 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5237 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7013 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2961 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2517 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8939 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3589 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2873 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      499 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/days.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      694 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/days_to_numbers.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      162 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/month_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      132 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/months.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      143 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/months_roman.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      198 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      100 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      353 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/electronic/symbols.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/fractions/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/fractions/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      150 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/fractions/fraction_symbols.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/inflection/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/inflection/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3803 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/inflection/endings.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      281 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/inflection/plural_endings.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      105 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/inflection/word_endings.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       81 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/math_operations.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/measures/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/measures/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      215 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/measures/greek_lower.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      215 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/measures/greek_upper.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      757 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/measures/measurements.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.091346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      278 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/money/alphabet.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      166 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/money/currency.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      106 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/money/currency_minor.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.095346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       68 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       66 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/digit_inline.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      111 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/digit_nom.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      250 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/quantities.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       94 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/tens.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       87 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/tens_inline.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        8 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.095346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      382 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/ordinals/endings.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       55 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/ordinals/exceptional.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       63 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/ordinals/superessive_endings.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       57 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/ordinals/superscript_digits.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.095346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      212 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/area_codes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      804 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/country_codes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       19 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/ip_prompt.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       44 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/special_numbers.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       29 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/telephone_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       10 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/telephone/telephone_prompt.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.095346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       87 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/time/time_zone.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      354 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/whitelist.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      548 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/whitelist_inflect.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      291 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/whitelist_inflect_sg.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1545 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.095346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12471 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10478 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5766 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3648 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2465 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5748 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7803 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3362 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6669 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11364 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7339 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3685 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1326 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5516 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.095346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1766 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2021 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2988 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3781 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2367 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2128 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3492 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1582 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2330 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3982 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3588 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2873 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    31001 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/normalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    22475 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/normalize_with_audio.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2891 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/preprocessing_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.095346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2077 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/alphabet.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.099346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.099346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/currency/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/currency/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1420 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1085 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.099346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       47 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      290 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      668 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      275 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/latin_to_cyrillic.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9277 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/measurements.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.099346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/months/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/months/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      239 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/months/abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1541 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      214 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/months/numbers.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.099346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      969 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      911 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      933 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      913 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1048 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      951 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      549 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      710 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      565 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1026 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      119 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/digits_nominative_case.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      430 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/ordinal_endings.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    21537 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      537 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.099346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      469 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_cardinal.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      611 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      828 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       62 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/time_convert.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.115346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3206 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/g.fst
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    69495 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)  7085564 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    14099 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1005 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/whitelist.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.119346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6818 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6014 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4465 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/decimals.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4796 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6942 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3997 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6605 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/number_names.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2950 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3265 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5253 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7139 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3044 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1312 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1287 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.119346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1891 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1497 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2189 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1570 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1759 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1494 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1462 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1782 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2115 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2993 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2925 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5055 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/run_evaluate.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.119346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.119346 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      334 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/abbreviations_nondet.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.123345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/dates/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/dates/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      116 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/dates/era_suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       94 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/dates/era_words.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      176 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/dates/month_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      112 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/dates/months.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.123345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/electronic/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/electronic/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/electronic/domain.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      289 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/electronic/server_name.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      263 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/electronic/symbols.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       71 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/math_operations.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.123345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      196 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/greek_lower.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      196 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/greek_upper.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2121 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      157 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/unit_neuter.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1461 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.123345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1344 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_major_nt.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      745 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      735 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1197 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.127345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       57 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      142 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/fraction.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1586 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/millions_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      330 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/quantities.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       94 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       72 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.127345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/ordinals/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/ordinals/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       83 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/ordinals/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      115 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/ordinals/teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       96 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/ordinals/ties.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        9 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/ordinals/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.127345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/roman/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/roman/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/roman/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/roman/hundreds.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       46 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/roman/ties.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.131345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      804 2023-06-08 22:44:38.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/country_codes.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       22 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/ip_prompt.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       96 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/special_numbers.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       28 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/ssn_prompt.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      381 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/telephone_abbr.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       58 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/telephone/telephone_prompt.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.131345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       53 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/time/hour_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       67 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/time/hour_to_night.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      336 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/time/minute_to.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      261 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/time/suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       64 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/time/time_zone.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1046 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/whitelist.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2520 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.131345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2167 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    17468 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     7019 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6751 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3466 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4169 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10129 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    12278 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9421 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8362 2023-06-06 22:35:18.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8752 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     9251 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    11094 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3023 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1322 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1173 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.135345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1732 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2631 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2837 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3678 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3155 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3749 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2806 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1584 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2379 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4270 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3589 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2872 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5164 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/token_parser.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    10972 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/utils_audio_based.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.135345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.135345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.135345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/charset_extension.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    32616 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      553 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       13 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/oov_tags.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      288 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/punctuations_zh.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       72 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/upper_to_lower.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.135345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/date/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/date/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       24 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/date/year_suffix.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.135345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/denylist/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        7 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/denylist/denylist.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.135345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/erhua/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      350 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/erhua/whitelist.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.139345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/math/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/math/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/math/score.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       52 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/math/symbol.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.139345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/measure/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/measure/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1138 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      988 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/measure/units_zh.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.139345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/money/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/money/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2374 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/money/currency_code.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1311 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/money/currency_symbol.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.139345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/number/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/number/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       54 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/number/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       51 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/number/digit_teen.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       12 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/number/sign.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        6 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/number/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.139345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       19 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/digit.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       63 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/hour.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      108 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/suffix.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       14 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/tens.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        2 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/zero.tsv
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.139345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/whitelist/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/whitelist/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      687 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/whitelist/default.tsv
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4046 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/graph_utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.143345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5168 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1087 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/char.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4010 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1491 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1652 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/math_symbol.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2079 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1789 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1850 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2678 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     4535 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1611 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1728 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.143345 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1190 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1100 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/char.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2847 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1458 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1139 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/math_symbol.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1885 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1379 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3046 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3481 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2813 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2222 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1289 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.007346 nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     5718 2023-06-13 19:48:45.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/PKG-INFO
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)    79163 2023-06-13 19:48:45.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/SOURCES.txt
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        1 2023-06-13 19:48:45.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/dependency_links.txt
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        1 2023-06-13 19:48:45.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/not-zip-safe
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      466 2023-06-13 19:48:45.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/requires.txt
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)       27 2023-06-13 19:48:45.000000 nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/top_level.txt
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.143345 nemo_text_processing-0.1.8rc0/requirements/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      139 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/requirements/requirements.txt
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      158 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/requirements/requirements_test.txt
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1142 2023-06-13 19:48:46.155345 nemo_text_processing-0.1.8rc0/setup.cfg
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8341 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/setup.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.143345 nemo_text_processing-0.1.8rc0/tests/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     8115 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/conftest.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.143345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.143345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-06-06 21:37:08.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1873 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2648 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2302 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2918 2023-06-13 19:46:44.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2374 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1954 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ar/test_whitelist.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.143345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2326 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2313 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2322 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2331 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2326 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2323 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2317 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1546 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_normalization_with_audio.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2046 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2329 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2313 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2329 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2314 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.147345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1885 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_address.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3053 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3752 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2950 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2943 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1785 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1842 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_math.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2931 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3030 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1530 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_normalization_with_audio.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2942 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1839 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_punctuation.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1847 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_range.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1852 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_roman.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1865 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_serial.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1956 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_special_text.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2962 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1748 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_text_split.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2928 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3635 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     3024 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.147345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2338 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2258 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2334 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2352 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1809 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2344 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2329 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1507 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_normalization_with_audio.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2335 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2349 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2334 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2347 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2396 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.147345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1282 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1279 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1285 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1282 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1276 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1274 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/data_text_normalization/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/data_text_normalization/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1243 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1235 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1241 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1247 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1244 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1242 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1238 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1242 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1246 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1235 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1245 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1235 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/hu/test_word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1282 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1279 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1285 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1276 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1280 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1273 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1284 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1274 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/data_text_normalization/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/data_text_normalization/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6340 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     6527 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/test_ru_normalization.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/__init__.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/data_text_normalization/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/data_text_normalization/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1793 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1786 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1791 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1797 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1794 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1792 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1788 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1602 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_normalization_with_audio.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1793 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1796 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1786 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1795 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1834 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_word.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     2812 2023-06-06 21:37:03.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/utils.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.151345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      610 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1600 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_cardinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1591 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1597 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_decimal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1603 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_electronic.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1600 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1598 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1594 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1598 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_ordinal.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1602 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_telephone.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1591 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_time.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1602 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_whitelist.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1592 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_word.py
+drwxrwxr-x   0 ebakhturina  (1000) ebakhturina  (1000)        0 2023-06-13 19:48:46.155345 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)      623 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/__init__.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1257 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_char.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1244 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_date.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1269 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_fraction.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1257 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_math.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1266 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_measure.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1230 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_money.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1275 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_preprocess.py
+-rw-rw-r--   0 ebakhturina  (1000) ebakhturina  (1000)     1257 2023-05-02 01:02:17.000000 nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_time.py
```

### Comparing `nemo_text_processing-0.1.7rc0/LICENSE` & `nemo_text_processing-0.1.8rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/PKG-INFO` & `nemo_text_processing-0.1.8rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo_text_processing
-Version: 0.1.7rc0
+Version: 0.1.8rc0
 Summary: NeMo text processing for ASR and TTS
 Home-page: https://github.com/nvidia/nemo-text-processing
 Download-URL: https://github.com/NVIDIA/NeMo-text-processing/releases
 Author: NVIDIA
 Author-email: nemo-toolkit@nvidia.com
 Maintainer: NVIDIA
 Maintainer-email: nemo-toolkit@nvidia.com
```

### Comparing `nemo_text_processing-0.1.7rc0/README.md` & `nemo_text_processing-0.1.8rc0/README.md`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/fst_alignment/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/fst_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/fst_alignment/alignment.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/fst_alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/mlm_scorer.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/mlm_scorer.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/model_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/model_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/hybrid/wfst_lm_rescoring.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/hybrid/wfst_lm_rescoring.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -49,11 +49,11 @@
         graph_integer = pynutil.insert('integer_part: "') + graph_integer_part + pynutil.insert('"')
         optional_graph_quantity = pynutil.insert('quantity: "') + optional_graph_quantity + pynutil.insert('"')
         optional_graph_quantity = pynini.closure(pynini.accep(NEMO_SPACE) + optional_graph_quantity, 0, 1)
 
         self.final_graph_wo_sign = (
             graph_integer + pynini.accep(NEMO_SPACE) + graph_fractional + optional_graph_quantity
         )
-        final_graph = optional_graph_negative + self.final_graph_wo_sign
+        self.final_graph_wo_negative = optional_graph_negative + self.final_graph_wo_sign
 
-        final_graph = self.add_tokens(final_graph)
+        final_graph = self.add_tokens(self.final_graph_wo_negative)
         self.fst = final_graph.optimize()
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,14 +15,15 @@
 import logging
 import os
 
 import pynini
 from nemo_text_processing.inverse_text_normalization.ar.taggers.cardinal import CardinalFst
 from nemo_text_processing.inverse_text_normalization.ar.taggers.decimal import DecimalFst
 from nemo_text_processing.inverse_text_normalization.ar.taggers.fraction import FractionFst
+from nemo_text_processing.inverse_text_normalization.ar.taggers.measure import MeasureFst
 from nemo_text_processing.inverse_text_normalization.ar.taggers.money import MoneyFst
 from nemo_text_processing.inverse_text_normalization.ar.taggers.punctuation import PunctuationFst
 from nemo_text_processing.inverse_text_normalization.ar.taggers.word import WordFst
 from nemo_text_processing.text_normalization.ar.graph_utils import (
     GraphFst,
     delete_extra_space,
     delete_space,
@@ -72,22 +73,30 @@
             cardinal_graph = cardinal.fst
             decimal = DecimalFst(tn_decimal=tn_classify.decimal)
             decimal_graph = decimal.fst
             fraction = FractionFst(tn_cardinal=tn_classify.cardinal)
             fraction_graph = fraction.fst
             money = MoneyFst(itn_cardinal_tagger=cardinal)
             money_graph = money.fst
+            measure = MeasureFst(
+                itn_cardinal_tagger=cardinal,
+                itn_decimal_tagger=decimal,
+                itn_fraction_tagger=fraction,
+                deterministic=True,
+            )
+            measure_graph = measure.fst
             word_graph = WordFst().fst
             punct_graph = PunctuationFst().fst
 
             classify = (
                 pynutil.add_weight(cardinal_graph, 1.1)
                 | pynutil.add_weight(decimal_graph, 1.1)
                 | pynutil.add_weight(fraction_graph, 1.1)
                 | pynutil.add_weight(money_graph, 1.1)
+                | pynutil.add_weight(measure_graph, 1.1)
                 | pynutil.add_weight(word_graph, 100)
             )
 
             punct = pynutil.insert("tokens { ") + pynutil.add_weight(punct_graph, weight=1.1) + pynutil.insert(" }")
             token = pynutil.insert("tokens { ") + classify + pynutil.insert(" }")
             token_plus_punct = (
                 pynini.closure(punct + pynutil.insert(" ")) + token + pynini.closure(pynutil.insert(" ") + punct)
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 # Copyright (c) 2023, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
-
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from nemo_text_processing.inverse_text_normalization.ar.verbalizers.cardinal import CardinalFst
-from nemo_text_processing.inverse_text_normalization.ar.verbalizers.decimal import DecimalFst
-from nemo_text_processing.inverse_text_normalization.ar.verbalizers.fraction import FractionFst
-from nemo_text_processing.inverse_text_normalization.ar.verbalizers.money import MoneyFst
 from nemo_text_processing.text_normalization.ar.graph_utils import GraphFst
+from nemo_text_processing.text_normalization.ar.taggers.cardinal import CardinalFst as CardinalTagger
+from nemo_text_processing.text_normalization.ar.verbalizers.cardinal import CardinalFst
+from nemo_text_processing.text_normalization.ar.verbalizers.decimal import DecimalFst
+from nemo_text_processing.text_normalization.ar.verbalizers.fraction import FractionFst
+from nemo_text_processing.text_normalization.ar.verbalizers.measure import MeasureFst
+from nemo_text_processing.text_normalization.ar.verbalizers.money import MoneyFst
 
 
 class VerbalizeFst(GraphFst):
     """
     Composes other verbalizer grammars.
     For deployment, this grammar will be compiled and exported to OpenFst Finite State Archive (FAR) File.
     More details to deployment at NeMo/tools/text_processing_deployment.
+
+    Args:
+        deterministic: if True will provide a single transduction option,
+            for False multiple options (used for audio-based normalization)
     """
 
-    def __init__(self):
-        super().__init__(name="verbalize", kind="verbalize")
+    def __init__(self, deterministic: bool = True):
+        super().__init__(name="verbalize", kind="verbalize", deterministic=deterministic)
+        cardinal_tagger = CardinalTagger()
         cardinal = CardinalFst()
         cardinal_graph = cardinal.fst
         decimal = DecimalFst()
         decimal_graph = decimal.fst
         fraction = FractionFst()
         fraction_graph = fraction.fst
-        money = MoneyFst(decimal, deterministic=True)
+        money = MoneyFst()
         money_graph = money.fst
-        graph = cardinal_graph | decimal_graph | fraction_graph | money_graph
+        measure = MeasureFst(decimal=decimal, cardinal=cardinal, fraction=fraction, deterministic=deterministic)
+        measure_graph = measure.fst
+
+        graph = cardinal_graph | decimal_graph | fraction_graph | money_graph | measure_graph
         self.fst = graph
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/de/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/clean_eval_data.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/currency.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             + delete_extra_space
             + month_graph
             + optional_graph_year
         )
 
         financial_period_graph = pynini.string_file(get_abs_path("data/date_period.tsv")).invert()
         period_fy = (
-            pynutil.insert("period: \"")
+            pynutil.insert("text: \"")
             + financial_period_graph
             + (pynini.cross(" ", "") | pynini.cross(" of ", ""))
             + pynutil.insert("\"")
         )
 
         graph_year = (
             pynutil.insert("year: \"") + (year_graph | _get_range_graph(input_case=input_case)) + pynutil.insert("\"")
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             + delete_space
             + pynutil.delete("\"")
             + pynini.closure(NEMO_NOT_QUOTE, 1)
             + delete_space
             + pynutil.delete("\"")
         )
         period = (
-            pynutil.delete("period:")
+            pynutil.delete("text:")
             + delete_space
             + pynutil.delete("\"")
             + pynini.closure(NEMO_NOT_QUOTE, 1)
             + pynutil.delete("\"")
         )
         graph_fy = period + pynini.closure(delete_extra_space + year, 0, 1)
         # month (day) year
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/en/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/g2p/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/g2p/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/fractions/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_plural_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_major_singular_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_plural_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/currency_minor_singular_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/teen.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/ordinals/twenties.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/time/time_zone_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/fractions.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/measurements/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/data/time/minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/graph_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import logging
 import os
 import string
 from pathlib import Path
 from typing import Dict
 
 import pynini
 from nemo_text_processing.inverse_text_normalization.fr.utils import get_abs_path
@@ -75,15 +76,15 @@
         file_name: exported file name
         graphs: Mapping of a rule name and Pynini WFST graph to be exported
     """
     exporter = export.Exporter(file_name)
     for rule, graph in graphs.items():
         exporter[rule] = graph.optimize()
     exporter.close()
-    print(f'Created {file_name}')
+    logging.info(f'Created {file_name}')
 
 
 def get_plurals(fst):
     """
     Given singular returns plurals
 
     Args:
@@ -106,15 +107,15 @@
     return PLURAL_TO_SINGULAR @ fst
 
 
 def convert_space(fst) -> 'pynini.FstLike':
     """
     Converts space to nonbreaking space.
     Used only in tagger grammars for transducing token values within quotes, e.g. name: "hello kitty"
-    This is making transducer significantly slower, so only use when there could be potential spaces within quotes, otherwise leave it. 
+    This is making transducer significantly slower, so only use when there could be potential spaces within quotes, otherwise leave it.
 
     Args:
         fst: input fst
 
     Returns output fst where breaking spaces are converted to non breaking spaces
     """
     return fst @ pynini.cdrewrite(pynini.cross(NEMO_SPACE, NEMO_NON_BREAKING_SPACE), "", "", NEMO_SIGMA)
@@ -155,17 +156,17 @@
     def fst(self, fst):
         self._fst = fst
 
     def add_tokens(self, fst) -> 'pynini.FstLike':
         """
         Wraps class name around to given fst
 
-        Args: 
+        Args:
             fst: input fst
-        
+
         Returns:
             Fst: fst
         """
         return pynutil.insert(f"{self.name} {{ ") + fst + pynutil.insert(" }")
 
     def delete_tokens(self, fst) -> 'pynini.FstLike':
         """
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/fr/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/inverse_normalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/inverse_normalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/measurements_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/pt/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ru/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/run_evaluate.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/run_evaluate.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/math/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/data/time/minutes.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/graph_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import logging
 import os
 import string
 from pathlib import Path
 from typing import Dict
 
 import pynini
 from pynini import Far
@@ -62,15 +63,15 @@
         file_name: exported file name
         graphs: Mapping of a rule name and Pynini WFST graph to be exported
     """
     exporter = export.Exporter(file_name)
     for rule, graph in graphs.items():
         exporter[rule] = graph.optimize()
     exporter.close()
-    print(f"Created {file_name}")
+    logging.info(f"Created {file_name}")
 
 
 def convert_space(fst) -> "pynini.FstLike":
     """
     Converts space to nonbreaking space.
     Used only in tagger grammars for transducing token values within quotes, e.g. name: "hello kitty"
     This is making transducer significantly slower, so only use when there could be potential spaces within quotes, otherwise leave it.
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/vi/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/package_info.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/package_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 MAJOR = 0
 MINOR = 1
-PATCH = 7
+PATCH = 8
 PRE_RELEASE = 'rc0'
 
 # Use the following formatting: (major, minor, patch, pre-release)
 VERSION = (MAJOR, MINOR, PATCH, PRE_RELEASE)
 
 __shortversion__ = '.'.join(map(str, VERSION[:3]))
 __version__ = '.'.join(map(str, VERSION[:3])) + ''.join(VERSION[3:])
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/es/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/data/number/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/graph_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import logging
 import os
 import string
 from pathlib import Path
 from typing import Dict
 
 from nemo_text_processing.text_normalization.en.utils import get_abs_path
 
@@ -205,15 +206,15 @@
         file_name: exported file name
         graphs: Mapping of a rule name and Pynini WFST graph to be exported
     """
     exporter = export.Exporter(file_name)
     for rule, graph in graphs.items():
         exporter[rule] = graph.optimize()
     exporter.close()
-    print(f'Created {file_name}')
+    logging.info(f'Created {file_name}')
 
 
 def get_plurals(fst):
     """
     Given singular returns plurals
 
     Args:
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,14 +23,15 @@
     delete_extra_space,
     delete_space,
     generator_main,
 )
 from nemo_text_processing.text_normalization.ar.taggers.cardinal import CardinalFst
 from nemo_text_processing.text_normalization.ar.taggers.decimal import DecimalFst
 from nemo_text_processing.text_normalization.ar.taggers.fraction import FractionFst
+from nemo_text_processing.text_normalization.ar.taggers.measure import MeasureFst
 from nemo_text_processing.text_normalization.ar.taggers.money import MoneyFst
 from nemo_text_processing.text_normalization.ar.taggers.word import WordFst
 from nemo_text_processing.text_normalization.en.taggers.punctuation import PunctuationFst
 from pynini.lib import pynutil
 
 
 class ClassifyFst(GraphFst):
@@ -76,22 +77,27 @@
             cardinal_graph = self.cardinal.fst
             self.decimal = DecimalFst(cardinal=self.cardinal, deterministic=deterministic)
             decimal_graph = self.decimal.fst
             self.fraction = FractionFst(cardinal=self.cardinal)
             fraction_graph = self.fraction.fst
             self.money = MoneyFst(cardinal=self.cardinal)
             money_graph = self.money.fst
+            self.measure = MeasureFst(
+                cardinal=self.cardinal, decimal=self.decimal, fraction=self.fraction, deterministic=deterministic
+            )
+            measure_graph = self.measure.fst
             word_graph = WordFst(deterministic=deterministic).fst
             punct_graph = PunctuationFst(deterministic=deterministic).fst
 
             classify = (
                 pynutil.add_weight(cardinal_graph, 1.1)
                 | pynutil.add_weight(decimal_graph, 1.1)
                 | pynutil.add_weight(fraction_graph, 1.0)
                 | pynutil.add_weight(money_graph, 1.0)
+                | pynutil.add_weight(measure_graph, 1.0)
             )
 
             classify |= pynutil.add_weight(word_graph, 100)
 
             punct = pynutil.insert("tokens { ") + pynutil.add_weight(punct_graph, weight=1.1) + pynutil.insert(" }")
             token = pynutil.insert("tokens { ") + classify + pynutil.insert(" }")
             token_plus_punct = (
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-# Copyright (c) 2022, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
+# Copyright (c) 2021, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from nemo_text_processing.text_normalization.ar.graph_utils import GraphFst
-from nemo_text_processing.text_normalization.ar.taggers.cardinal import CardinalFst as CardinalTagger
-from nemo_text_processing.text_normalization.ar.verbalizers.cardinal import CardinalFst
-from nemo_text_processing.text_normalization.ar.verbalizers.decimal import DecimalFst
-from nemo_text_processing.text_normalization.ar.verbalizers.fraction import FractionFst
-from nemo_text_processing.text_normalization.ar.verbalizers.money import MoneyFst
+from nemo_text_processing.text_normalization.en.graph_utils import GraphFst
+from nemo_text_processing.text_normalization.en.verbalizers.whitelist import WhiteListFst
+from nemo_text_processing.text_normalization.ru.verbalizers.cardinal import CardinalFst
+from nemo_text_processing.text_normalization.ru.verbalizers.date import DateFst
+from nemo_text_processing.text_normalization.ru.verbalizers.decimal import DecimalFst
+from nemo_text_processing.text_normalization.ru.verbalizers.electronic import ElectronicFst
+from nemo_text_processing.text_normalization.ru.verbalizers.measure import MeasureFst
+from nemo_text_processing.text_normalization.ru.verbalizers.money import MoneyFst
+from nemo_text_processing.text_normalization.ru.verbalizers.ordinal import OrdinalFst
+from nemo_text_processing.text_normalization.ru.verbalizers.telephone import TelephoneFst
+from nemo_text_processing.text_normalization.ru.verbalizers.time import TimeFst
 
 
 class VerbalizeFst(GraphFst):
     """
     Composes other verbalizer grammars.
     For deployment, this grammar will be compiled and exported to OpenFst Finite State Archive (FAR) File.
     More details to deployment at NeMo/tools/text_processing_deployment.
@@ -29,19 +34,36 @@
     Args:
         deterministic: if True will provide a single transduction option,
             for False multiple options (used for audio-based normalization)
     """
 
     def __init__(self, deterministic: bool = True):
         super().__init__(name="verbalize", kind="verbalize", deterministic=deterministic)
-        cardinal_tagger = CardinalTagger()
         cardinal = CardinalFst()
         cardinal_graph = cardinal.fst
+        ordinal_graph = OrdinalFst().fst
         decimal = DecimalFst()
         decimal_graph = decimal.fst
-        fraction = FractionFst()
-        fraction_graph = fraction.fst
-        money = MoneyFst()
-        money_graph = money.fst
-
-        graph = cardinal_graph | decimal_graph | fraction_graph | money_graph
+        date = DateFst()
+        date_graph = date.fst
+        measure = MeasureFst()
+        measure_graph = measure.fst
+        electronic = ElectronicFst()
+        electronic_graph = electronic.fst
+        whitelist_graph = WhiteListFst().fst
+        money_graph = MoneyFst().fst
+        telephone_graph = TelephoneFst().fst
+        time_graph = TimeFst().fst
+
+        graph = (
+            measure_graph
+            | cardinal_graph
+            | decimal_graph
+            | ordinal_graph
+            | date_graph
+            | electronic_graph
+            | money_graph
+            | whitelist_graph
+            | telephone_graph
+            | time_graph
+        )
         self.fst = graph
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ar/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/data_loader_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/data_loader_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/fractions.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/fractions.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/measure/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/measure/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/months/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/months/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/clean_eval_data.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/clean_eval_data.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/address/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/de/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/address/state.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/address/state.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/date/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/date/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/unit.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/unit.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/measure/unit_alternatives.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/number/cardinal_number_name_au.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/ordinal/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/female.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/female.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/male.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/male.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/roman/roman_to_spoken.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/suppletive.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/suppletive.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/telephone/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/telephone/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/alternatives.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/asr_with_pc.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/ipa_symbols.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/whitelist/tts.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/graph_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import logging
 import os
 import string
 from pathlib import Path
 from typing import Dict
 
 import pynini
 from nemo_text_processing.text_normalization.en.utils import get_abs_path, load_labels
@@ -135,15 +136,15 @@
         file_name: exported file name
         graphs: Mapping of a rule name and Pynini WFST graph to be exported
     """
     exporter = export.Exporter(file_name)
     for rule, graph in graphs.items():
         exporter[rule] = graph.optimize()
     exporter.close()
-    print(f'Created {file_name}')
+    logging.info(f'Created {file_name}')
 
 
 def get_plurals(fst):
     """
     Given singular returns plurals
 
     Args:
@@ -196,15 +197,15 @@
                     ],  # # add pairs with the all letters capitalized
                 ]
             )
 
             spoken_no_space = spoken.replace(" ", "")
             # add abbreviations without spaces (both lower and upper case), i.e. "BMW" not "B M W"
             if len(spoken) == (2 * len(spoken_no_space) - 1):
-                print(f"This is weight {weight}")
+                logging.debug(f"This is weight {weight}")
                 if len(weight) == 0:
                     additional_labels.extend(
                         [[written, spoken_no_space], [written_capitalized, spoken_no_space.upper()]]
                     )
                 else:
                     additional_labels.extend(
                         [
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/abbreviation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/abbreviation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
                 + pynini.closure(pynutil.delete("0"), 0, 1)
                 + day_graph
             )
             final_graph |= m_sep_d
         else:
             final_graph += pynutil.insert(" preserve_order: true")
 
-        period_fy = pynutil.insert("period: \"") + _get_financial_period_graph() + pynutil.insert("\"")
+        period_fy = pynutil.insert("text: \"") + _get_financial_period_graph() + pynutil.insert("\"")
         graph_fy = period_fy + insert_space + two_digit_year
 
         final_graph |= graph_ymd | year_graph | graph_fy
 
         if not deterministic or lm:
             ymd_to_mdy_graph = None
             ymd_to_dmy_graph = None
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/electronic.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import pynini
 from nemo_text_processing.text_normalization.en.graph_utils import (
     MIN_NEG_WEIGHT,
     NEMO_ALPHA,
     NEMO_DIGIT,
     NEMO_NOT_SPACE,
+    NEMO_SIGMA,
     NEMO_UPPER,
     TO_UPPER,
     GraphFst,
     get_abs_path,
     insert_space,
 )
 from pynini.lib import pynutil
@@ -94,15 +95,18 @@
                 domain_graph,
             ).optimize()
             + pynutil.insert("\"")
         )
 
         protocol = pynutil.insert("protocol: \"") + pynutil.add_weight(protocol, MIN_NEG_WEIGHT) + pynutil.insert("\"")
         # email
-        graph = username + domain_graph_with_class_tags
+        graph = pynini.compose(
+            NEMO_SIGMA + pynini.accep("@") + NEMO_SIGMA + pynini.accep(".") + NEMO_SIGMA,
+            username + domain_graph_with_class_tags,
+        )
 
         # abc.com, abc.com/123-sm
         # when only domain, make sure it starts and end with NEMO_ALPHA
         graph |= (
             pynutil.insert("domain: \"")
             + pynini.compose(
                 NEMO_ALPHA + pynini.closure(NEMO_NOT_SPACE) + accepted_common_domains + pynini.closure(NEMO_NOT_SPACE),
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/punctuation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/range.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/range.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/roman.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/roman.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/serial.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/serial.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_lm.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/tokenize_and_classify_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/abbreviation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             pynutil.delete("day:")
             + delete_space
             + pynutil.delete("\"")
             + pynini.closure(NEMO_NOT_QUOTE, 1)
             + pynutil.delete("\"")
         )
         day = day_cardinal @ ordinal.suffix
-        period = pynutil.delete("period:") + delete_space + pynutil.delete("\"") + phrase + pynutil.delete("\"")
+        period = pynutil.delete("text:") + delete_space + pynutil.delete("\"") + phrase + pynutil.delete("\"")
         month = pynutil.delete("month:") + delete_space + pynutil.delete("\"") + phrase + pynutil.delete("\"")
 
         year = (
             pynutil.delete("year:")
             + delete_space
             + pynutil.delete("\"")
             + pynini.closure(NEMO_NOT_QUOTE, 1)
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/post_processing.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/roman.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/roman.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/en/verbalizers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/verbalizers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/months_abbr.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/dates/year_suffix.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/fractions/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/fractions/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/measures/measurements_plural_masc.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_major_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_minor_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_fem_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/money/currency_plural_masc_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/roman/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/telephone/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/time_zone.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/time/time_zone_ext.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/data/whitelist.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/decimals.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/decimals.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,22 +78,23 @@
         if not deterministic:
             graph = pynini.union(graph_digit, cardinal.hundreds, cardinal.tens)
             graph += pynini.closure(insert_space + graph)
 
         else:
             # General pattern is 1-3 digits: map as cardinal, default to tens followed by digits otherwise \
             graph = pynini.union(
-                graph_digit + pynini.closure(insert_space + zero),
-                cardinal.tens + pynini.closure(insert_space + zero),
-                cardinal.hundreds + pynini.closure(insert_space + zero),
-                cardinal.tens
-                + pynini.closure(insert_space + cardinal.tens, 1)
-                + pynini.closure(insert_space + zero, 0, 1)
-                + (
-                    pynini.closure(insert_space + graph_digit, 0, 1) | pynini.closure(insert_space + zero, 0)
+                pynutil.add_weight(graph_digit + pynini.closure(insert_space + zero), -0.00001),
+                pynutil.add_weight(cardinal.tens + pynini.closure(insert_space + zero), -0.00002),
+                pynutil.add_weight(cardinal.hundreds + pynini.closure(insert_space + zero), 0.00001),
+                pynutil.add_weight(
+                    cardinal.tens
+                    + pynini.closure(insert_space + cardinal.tens, 1)
+                    + pynini.closure(insert_space + zero, 0, 1)
+                    + (pynini.closure(insert_space + graph_digit, 0, 1) | pynini.closure(insert_space + zero, 0)),
+                    -0.00002,
                 ),  # Read out as tens and a possible trailing digit or zeroes
                 zero
                 + pynini.closure(insert_space + zero)
                 + pynini.closure(insert_space + graph_digit),  # For cases such as "1,010"
             )
 
         # Need to strip apocope everywhere BUT end of string
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/measure.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pynini
 from nemo_text_processing.text_normalization.en.graph_utils import (
     NEMO_ALPHA,
-    NEMO_DIGIT,
     NEMO_NON_BREAKING_SPACE,
     NEMO_SIGMA,
     NEMO_SPACE,
     GraphFst,
     convert_space,
     delete_space,
     insert_space,
@@ -49,27 +48,26 @@
         cardinal: CardinalFst
         decimal: DecimalFst
         fraction: FractionFst
         deterministic: if True will provide a single transduction option,
             for False multiple transduction are generated (used for audio-based normalization)
     """
 
-    def __init__(
-        self, cardinal: GraphFst, decimal: GraphFst, fraction: GraphFst, deterministic: bool = True,
-    ):
+    def __init__(self, cardinal: GraphFst, decimal: GraphFst, fraction: GraphFst, deterministic: bool = True):
         super().__init__(name="measure", kind="classify", deterministic=deterministic)
         cardinal_graph = cardinal.graph
-        optional_graph_negative = pynini.closure("-", 0, 1)
 
         unit_singular = unit
         unit_plural = unit_singular @ (unit_plural_fem | unit_plural_masc)
 
         graph_unit_singular = convert_space(unit_singular)
         graph_unit_plural = convert_space(unit_plural)
 
+        optional_graph_negative = pynini.closure("-", 0, 1)
+
         unit_plural = pynutil.insert('units: "') + graph_unit_plural + pynutil.insert('"')
 
         unit_singular_graph = pynutil.insert('units: "') + graph_unit_singular + pynutil.insert('"')
 
         unit_complex_plural = unit_complex @ (unit_plural_fem | unit_plural_masc)
 
         graph_unit_complex = convert_space(unit_complex)
@@ -94,86 +92,33 @@
             + ((graph_unit_plural + optional_unit_denominator) | graph_unit_denominator | graph_unit_complex_plural)
             + pynutil.insert('"')
         )
 
         subgraph_decimal = (
             decimal.fst + insert_space + pynini.closure(NEMO_SPACE, 0, 1) + (unit_plural | complex_unit_plural_graph)
         )
-
         subgraph_cardinal = (
             (optional_graph_negative + (NEMO_SIGMA - "1")) @ cardinal.fst
             + insert_space
             + pynini.closure(delete_space, 0, 1)
             + (unit_plural | complex_unit_plural_graph)
         )
 
         subgraph_cardinal |= (
             (optional_graph_negative + pynini.accep("1")) @ cardinal.fst
             + insert_space
             + pynini.closure(delete_space, 0, 1)
-            + (unit_plural | complex_unit_singular_graph)
-        )
-
-        """transform "1 1/2 km" ->  measure { cardinal { integer: "uno" } 
-                                    fraction { numerator: "un" denominator: "medio" morphosyntactic_features: "ordinal" } 
-                                    units: "kilómetro" } }
-        """
-        int_before_fraction = pynutil.add_weight(
-            (optional_graph_negative + pynini.accep("1")) @ cardinal.fst
-            + insert_space
-            + pynini.closure(delete_space, 0, 1),
-            -0.002,
-        )
-
-        subgraph_fraction = pynutil.add_weight(
-            pynini.closure(int_before_fraction, 0, 1)
-            + fraction.fst
-            + insert_space
-            + pynini.closure(delete_space, 0, 1)
-            + unit_singular_graph,
-            -0.002,
+            + (unit_singular_graph | complex_unit_singular_graph)
         )
 
-        """transform "2 1/2 km" ->  measure { cardinal { integer: "dos" } 
-                                    fraction { numerator: "un" denominator: "medio" morphosyntactic_features: "ordinal" } 
-                                    units: "kilómetros" } }
-        """
-        ints_before_fraction = (
-            (optional_graph_negative + (NEMO_SIGMA - "1")) @ cardinal.fst
-            + insert_space
-            + pynini.closure(delete_space, 0, 1)
-        )
-
-        subgraph_fraction |= pynutil.add_weight(
-            ints_before_fraction + fraction.fst + insert_space + pynini.closure(delete_space, 0, 1) + unit_plural,
-            -0.002,
-        )
-
-        """transform "2 1/2 k/h" -> measure { fraction { integer_part: "dos" 
-                                                         numerator: "un" 
-                                                         denominator: "medio" 
-                                                         morphosyntactic_features: "ordinal" } 
-                                              units: "kilómetros" } }
-        """
-        proper_fraction = pynini.closure(NEMO_DIGIT) + pynini.accep("/") + pynini.closure(NEMO_DIGIT)
-        subgraph_complex_units = pynutil.add_weight(
-            (proper_fraction @ fraction.fst)
+        subgraph_fraction = (
+            fraction.fst
             + insert_space
             + pynini.closure(delete_space, 0, 1)
-            + complex_unit_singular_graph
-            + pynutil.insert(' preserve_order: true'),
-            -0.001,
-        )
-
-        subgraph_complex_units |= (
-            ((NEMO_SIGMA - proper_fraction) @ fraction.fst)
-            + insert_space
-            + pynini.closure(delete_space, 0, 1)
-            + complex_unit_plural_graph
-            + pynutil.insert(' preserve_order: true')
+            + (unit_plural | complex_unit_singular_graph)
         )
 
         decimal_times = (
             pynutil.insert("decimal { ")
             + decimal.final_graph_wo_negative
             + pynutil.insert(' } units: "')
             + pynini.union("x", "X")
@@ -199,15 +144,15 @@
 
         decimal_dash_alpha = (
             pynutil.insert("decimal { ")
             + decimal.final_graph_wo_negative
             + pynutil.delete("-")
             + pynutil.insert(' } units: "')
             + pynini.closure(NEMO_ALPHA, 1)
-            + pynutil.insert('"')
+            + pynutil.insert("\"")
         )
 
         alpha_dash_cardinal = (
             pynutil.insert('units: "')
             + pynini.closure(NEMO_ALPHA, 1)
             + pynutil.delete("-")
             + pynutil.insert('"')
@@ -251,15 +196,14 @@
             + pynutil.insert("\" } preserve_order: true")
         )
 
         final_graph = (
             subgraph_decimal
             | subgraph_cardinal
             | cardinal_dash_alpha
-            | subgraph_complex_units
             | alpha_dash_cardinal
             | decimal_dash_alpha
             | subgraph_fraction
             | decimal_times
             | cardinal_times
             | alpha_dash_decimal
             | math
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,69 +41,69 @@
     """
 
     def __init__(self, cardinal: GraphFst, deterministic: bool = True):
         super().__init__(name="time", kind="classify", deterministic=deterministic)
 
         delete_time_delimiter = pynutil.delete(pynini.union(".", ":"))
 
-        one = pynini.string_map([("un", "una"), ("ún", "una")])
-        change_one = pynini.cdrewrite(one, "", "", NEMO_SIGMA)
-        cardinal_graph = cardinal.graph @ change_one
+        fem_one = pynini.string_map([("un", "una"), ("ún", "una")])
+        change_one = pynini.cdrewrite(fem_one, "", "", NEMO_SIGMA)
+        cardinal_graph_fem = cardinal.graph @ change_one
+        cardinal_graph_masc = cardinal.graph
 
         day_suffix = pynutil.insert("suffix: \"") + suffix + pynutil.insert("\"")
         day_suffix = delete_space + insert_space + day_suffix
 
         delete_hora_suffix = delete_space + insert_space + pynutil.delete("h")
-        delete_minute_suffix = delete_space + insert_space + pynutil.delete("min")
-        delete_second_suffix = delete_space + insert_space + pynutil.delete("s")
+        delete_minute_suffix = delete_space + insert_space + (pynutil.delete("min") | pynutil.delete("m"))
+        delete_second_suffix = delete_space + insert_space + (pynutil.delete("seg") | pynutil.delete("s"))
 
         labels_hour_24 = [
             str(x) for x in range(0, 25)
         ]  # Can see both systems. Twelve hour requires am/pm for ambiguity resolution
         labels_hour_12 = [str(x) for x in range(1, 13)]
-        labels_minute_single = [str(x) for x in range(1, 10)]
-        labels_minute_double = [str(x) for x in range(10, 60)]
+        labels_minute_or_second = [str(x) for x in range(1, 60)]
 
         delete_leading_zero_to_double_digit = (
             pynini.closure(pynutil.delete("0") | (NEMO_DIGIT - "0"), 0, 1) + NEMO_DIGIT
         )
 
         graph_24 = (
             pynini.closure(NEMO_DIGIT, 1, 2) @ delete_leading_zero_to_double_digit @ pynini.union(*labels_hour_24)
         )
         graph_12 = (
             pynini.closure(NEMO_DIGIT, 1, 2) @ delete_leading_zero_to_double_digit @ pynini.union(*labels_hour_12)
         )
-
-        graph_hour_24 = graph_24 @ cardinal_graph
-        graph_hour_12 = graph_12 @ cardinal_graph
-
-        graph_minute_single = (NEMO_DIGIT | pynutil.delete("0")) + NEMO_DIGIT @ pynini.union(*labels_minute_single)
-        graph_minute_double = pynini.union(*labels_minute_double)
-
-        graph_minute = pynini.union(graph_minute_single, graph_minute_double) @ cardinal_graph
+        graph_minute_or_second = (
+            pynini.closure(NEMO_DIGIT, 1, 2)
+            @ delete_leading_zero_to_double_digit
+            @ pynini.union(*labels_minute_or_second)
+        )
+        graph_hour_24 = graph_24 @ cardinal_graph_fem
+        graph_hour_12 = graph_12 @ cardinal_graph_fem
+        graph_minute_or_second @= cardinal_graph_masc
 
         final_graph_hour_only_24 = (
             pynutil.insert("hours: \"") + graph_hour_24 + pynutil.insert("\"") + delete_hora_suffix
         )
         final_graph_hour_only_12 = pynutil.insert("hours: \"") + graph_hour_12 + pynutil.insert("\"") + day_suffix
 
         final_graph_hour_24 = pynutil.insert("hours: \"") + graph_hour_24 + pynutil.insert("\"")
         final_graph_hour_12 = pynutil.insert("hours: \"") + graph_hour_12 + pynutil.insert("\"")
 
-        final_graph_minute = pynutil.insert("minutes: \"") + graph_minute + pynutil.insert("\"")
-        final_graph_second = pynutil.insert("seconds: \"") + graph_minute + pynutil.insert("\"")
+        final_graph_minute = pynutil.insert("minutes: \"") + graph_minute_or_second + pynutil.insert("\"")
+        final_graph_second = pynutil.insert("seconds: \"") + graph_minute_or_second + pynutil.insert("\"")
 
         # handle suffixes like gmt or utc+1
         utc_one = pynini.string_map([("un", "uno"), ("ún", "uno")])
         change_utc_one = pynini.cdrewrite(utc_one, "", "", NEMO_SIGMA)
         utc_cardinal_graph = cardinal.graph @ change_utc_one
 
         utc_or_gmt_numbers = (NEMO_DIGIT @ utc_cardinal_graph) | (
-            graph_hour_24 + delete_time_delimiter + pynutil.insert(" ") + graph_minute
+            graph_hour_24 + delete_time_delimiter + pynutil.insert(" ") + graph_minute_or_second
         )
 
         utc_or_gmt_diff = (
             pynutil.delete(pynini.closure(" ", 0, 1))
             + pynutil.insert(" ")
             + pynini.string_map([("+", "más"), ("-", "menos")])
             + pynutil.delete(pynini.closure(" ", 0, 1))
@@ -119,67 +119,61 @@
 
         # 02.30 h
         graph_hm = (
             final_graph_hour_24
             + delete_time_delimiter
             + (pynutil.delete("00") | (insert_space + final_graph_minute))
             + pynini.closure(
-                delete_time_delimiter + (pynini.cross("00", " seconds: \"0\"") | (insert_space + final_graph_second)),
-                0,
-                1,
-            )  # For seconds 2.30.35 h
+                (delete_time_delimiter + (pynutil.delete("00") | (insert_space + final_graph_second))), 0, 1
+            )
             + pynini.closure(delete_hora_suffix, 0, 1)  # 2.30 is valid if unambiguous
             + final_time_zone_optional
         )
 
         # 2 h 30 min
         graph_hm |= (
             final_graph_hour_24
             + delete_hora_suffix
             + delete_space
             + (pynutil.delete("00") | (insert_space + final_graph_minute))
             + delete_minute_suffix
             + pynini.closure(
-                delete_space
-                + (pynini.cross("00", " seconds: \"0\"") | (insert_space + final_graph_second))
-                + delete_second_suffix,
+                (delete_space + (pynutil.delete("00") | (insert_space + final_graph_second)) + delete_second_suffix),
                 0,
                 1,
-            )  # For seconds
+            )
             + final_time_zone_optional
         )
 
         # 2.30 a. m. (Only for 12 hour clock)
         graph_hm |= (
             final_graph_hour_12
             + delete_time_delimiter
             + (pynutil.delete("00") | (insert_space + final_graph_minute))
             + pynini.closure(
-                delete_time_delimiter + (pynini.cross("00", " seconds: \"0\"") | (insert_space + final_graph_second)),
-                0,
-                1,
-            )  # For seconds 2.30.35 a. m.
+                (delete_time_delimiter + (pynutil.delete("00") | (insert_space + final_graph_second))), 0, 1
+            )
             + day_suffix
             + final_time_zone_optional
         )
 
         graph_h = (
             pynini.union(final_graph_hour_only_24, final_graph_hour_only_12) + final_time_zone_optional
         )  # Should always have a time indicator, else we'll pass to cardinals
 
         if not deterministic:
             # This includes alternate vocalization (hour menos min, min para hour), here we shift the times and indicate a `style` tag
             hour_shift_24 = pynini.invert(pynini.string_file(get_abs_path("data/time/hour_to_24.tsv")))
             hour_shift_12 = pynini.invert(pynini.string_file(get_abs_path("data/time/hour_to_12.tsv")))
             minute_shift = pynini.string_file(get_abs_path("data/time/minute_to.tsv"))
 
-            graph_hour_to_24 = graph_24 @ hour_shift_24 @ cardinal_graph
-            graph_hour_to_12 = graph_12 @ hour_shift_12 @ cardinal_graph
+            graph_hour_to_24 = graph_24 @ hour_shift_24 @ cardinal_graph_fem
+            graph_hour_to_12 = graph_12 @ hour_shift_12 @ cardinal_graph_fem
 
-            graph_minute_to = pynini.union(graph_minute_single, graph_minute_double) @ minute_shift @ cardinal_graph
+            graph_minute_to = minute_shift @ graph_minute_or_second
 
             final_graph_hour_to_24 = pynutil.insert("hours: \"") + graph_hour_to_24 + pynutil.insert("\"")
             final_graph_hour_to_12 = pynutil.insert("hours: \"") + graph_hour_to_12 + pynutil.insert("\"")
 
             final_graph_minute_to = pynutil.insert("minutes: \"") + graph_minute_to + pynutil.insert("\"")
 
             graph_menos = pynutil.insert(" style: \"1\"")
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/tokenize_and_classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 | pynutil.add_weight(time_graph, 1.09)
                 | pynutil.add_weight(measure_graph, 1.08)
                 | pynutil.add_weight(cardinal_graph, 1.1)
                 | pynutil.add_weight(fraction_graph, 1.09)
                 | pynutil.add_weight(date_graph, 1.1)
                 | pynutil.add_weight(ordinal_graph, 1.1)
                 | pynutil.add_weight(decimal_graph, 1.1)
-                | pynutil.add_weight(money_graph, 1.1)
+                | pynutil.add_weight(money_graph, 1.09)
                 | pynutil.add_weight(telephone_graph, 1.11)
                 | pynutil.add_weight(electronic_graph, 1.1)
                 | pynutil.add_weight(word_graph, 200)
             )
             punct = pynutil.insert("tokens { ") + pynutil.add_weight(punct_graph, weight=2.1) + pynutil.insert(" }")
             punct = pynini.closure(
                 pynini.compose(pynini.closure(NEMO_WHITE_SPACE, 1), delete_extra_space)
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/decimals.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/measure.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,50 +68,20 @@
 
         unit_fem = (unit_plural_fem | unit_singular_fem) + pynini.closure(
             NEMO_WHITE_SPACE + "por" + pynini.closure(NEMO_NOT_QUOTE, 1), 0, 1
         )
         unit_fem = pynutil.delete("units: \"") + (pynini.closure(NEMO_NOT_QUOTE) @ unit_fem) + pynutil.delete("\"")
 
         graph_masc = (graph_cardinal_masc | graph_decimal_masc) + NEMO_WHITE_SPACE + unit_masc
-        graph_masc |= pynutil.add_weight(
-            graph_cardinal_masc
-            + NEMO_WHITE_SPACE
-            + unit_masc
-            + NEMO_WHITE_SPACE
-            + pynutil.insert("y ")
-            + pynutil.delete(" ")
-            + graph_fraction_masc,
-            -0.002,
-        )  # "dos metros y medio" not "dos y medio metro"
         graph_masc |= graph_fraction_masc + NEMO_WHITE_SPACE + pynutil.insert("de ") + unit_masc
         graph_masc |= pynutil.add_weight(
             graph_fraction_masc @ (NEMO_SIGMA + pynini.union("medio", "medios")) + NEMO_WHITE_SPACE + unit_masc, -0.001
         )  # "medio litro" not "medio de litro"
 
         graph_fem = (graph_cardinal_fem | graph_decimal_fem) + NEMO_WHITE_SPACE + unit_fem
-        graph_fem |= pynutil.add_weight(
-            graph_cardinal_fem
-            + NEMO_WHITE_SPACE
-            + unit_fem
-            + NEMO_WHITE_SPACE
-            + pynutil.insert("y ")
-            + pynutil.delete(" ")
-            + graph_fraction_fem,
-            -0.002,
-        )
-        graph_fem |= pynutil.add_weight(
-            graph_cardinal_fem
-            + NEMO_WHITE_SPACE
-            + unit_fem
-            + NEMO_WHITE_SPACE
-            + pynutil.insert("y ")
-            + pynutil.delete(" ")
-            + graph_fraction_fem @ (NEMO_SIGMA + pynini.accep("media")),
-            -0.003,
-        )
         graph_fem |= graph_fraction_fem + NEMO_WHITE_SPACE + pynutil.insert("de ") + unit_fem
         graph_fem |= pynutil.add_weight(
             graph_fraction_fem @ (NEMO_SIGMA + pynini.union("media", "medias")) + NEMO_WHITE_SPACE + unit_fem, -0.001
         )
 
         graph = graph_masc | graph_fem
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/normalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,25 +134,29 @@
             from nemo_text_processing.text_normalization.de.verbalizers.verbalize_final import VerbalizeFinalFst
         elif lang == 'es':
             from nemo_text_processing.text_normalization.es.taggers.tokenize_and_classify import ClassifyFst
             from nemo_text_processing.text_normalization.es.verbalizers.verbalize_final import VerbalizeFinalFst
         elif lang == 'sv':
             from nemo_text_processing.text_normalization.sv.taggers.tokenize_and_classify import ClassifyFst
             from nemo_text_processing.text_normalization.sv.verbalizers.verbalize_final import VerbalizeFinalFst
+        elif lang == 'hu':
+            from nemo_text_processing.text_normalization.hu.taggers.tokenize_and_classify import ClassifyFst
+            from nemo_text_processing.text_normalization.hu.verbalizers.verbalize_final import VerbalizeFinalFst
         elif lang == 'zh':
             from nemo_text_processing.text_normalization.zh.taggers.tokenize_and_classify import ClassifyFst
             from nemo_text_processing.text_normalization.zh.verbalizers.verbalize_final import VerbalizeFinalFst
         elif lang == 'ar':
             from nemo_text_processing.text_normalization.ar.taggers.tokenize_and_classify import ClassifyFst
             from nemo_text_processing.text_normalization.ar.verbalizers.verbalize_final import VerbalizeFinalFst
         else:
             raise NotImplementedError(f"Language {lang} has not been supported yet.")
 
+        self.input_case = input_case
         self.tagger = ClassifyFst(
-            input_case=input_case,
+            input_case=self.input_case,
             deterministic=deterministic,
             cache_dir=cache_dir,
             overwrite_cache=overwrite_cache,
             whitelist=whitelist,
         )
 
         self.verbalizer = VerbalizeFinalFst(
@@ -502,15 +506,15 @@
         # end of quoted speech - to be able to split sentences by full stop
         text = re.sub(r"([\.\?\!])([\"\'])", r"\g<2>\g<1> ", text)
 
         # remove extra space
         text = re.sub(r" +", " ", text)
 
         # remove space in the middle of the lower case abbreviation to avoid splitting into separate sentences
-        matches = re.findall(r"[a-z" + lower_case_unicode + "]\.\s[a-z" + lower_case_unicode + "]\.", text)
+        matches = re.findall(rf"[a-z{lower_case_unicode}]\.\s[a-z{lower_case_unicode}]\.", text)
         for match in matches:
             text = text.replace(match, match.replace(". ", "."))
 
         # Read and split transcript by utterance (roughly, sentences)
         split_pattern = rf"(?<!\w\.\w.)(?<![A-Z{upper_case_unicode}][a-z{lower_case_unicode}]+\.)(?<![A-Z{upper_case_unicode}]\.)(?<=\.|\?|\!|\.”|\?”\!”)\s(?![0-9]+[a-z]*\.)"
         sentences = regex.split(split_pattern, text)
         sentences = additional_split(sentences, additional_split_symbols)
@@ -663,15 +667,15 @@
         '--manifest_text_field',
         help="A field in .json manifest to normalize (applicable only when input_file is a .json manifest)",
         type=str,
         default="text",
     )
     parser.add_argument('--output_file', dest="output_file", help="Output file path", type=str)
     parser.add_argument(
-        "--language", help="language", choices=["en", "de", "es", "sv", "zh", "ar"], default="en", type=str
+        "--language", help="language", choices=["en", "de", "es", "hu", "sv", "zh", "ar"], default="en", type=str
     )
     parser.add_argument(
         "--input_case",
         help="Input text capitalization, set to 'cased' if text contains capital letters."
         "This flag affects normalization rules applied to the text. Note, `lower_cased` won't lower case input.",
         choices=["lower_cased", "cased"],
         default="cased",
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/normalize_with_audio.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/normalize_with_audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import json
 import os
 from argparse import ArgumentParser
 from time import perf_counter
 from typing import List, Optional, Tuple
 
-import jiwer
+import editdistance
 import pynini
 from nemo_text_processing.text_normalization.data_loader_utils import post_process_punct, pre_process
 from nemo_text_processing.text_normalization.normalize import Normalizer
 from nemo_text_processing.text_normalization.utils_audio_based import get_alignment
 from pynini.lib import rewrite
 
 
@@ -402,15 +402,15 @@
     normalized_options = []
     for i, text in enumerate(normalized_texts):
         text_clean = text.replace('-', ' ').lower()
         if remove_punct:
             for punct in "!?:;,.-()*+-/<=>@^_":
                 text_clean = text_clean.replace(punct, " ").replace("  ", " ")
 
-        cer = jiwer.cer(pred_text, text_clean) * 100
+        cer = editdistance.eval(pred_text, text_clean) * 100.0 / len(pred_text)
         normalized_options.append((text, cer, i))
     return normalized_options
 
 
 def parse_args():
     parser = ArgumentParser()
     parser.add_argument("--text", help="input string or path to a .txt file", default=None, type=str)
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/preprocessing_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/alphabet.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/alphabet.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/currency/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/currency/currency_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/electronic/symbols.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/measurements.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/measurements.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/months/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/months/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/months/abbr_to_name.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/1_cardinals_nominative.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/2_cardinals_genitive.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/3_cardinals_dative.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/4_cardinals_accusative.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/5_cardinals_instrumental.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/6_cardinals_prepositional.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_alternatives.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/cardinals_nominative_case.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_delimiter.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/decimal_endings.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/ordinals.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/numbers/quantity.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/increment_hour_ordinal.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/time/minutes_to_hour.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/g.fst` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/g.fst`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/universal_thousands_punct.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/util_arithmetic.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/utils/util_byte.far`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/data/whitelist.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/decimals.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/number_names.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/number_names.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,44 @@
-# Copyright (c) 2021, NVIDIA CORPORATION.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION & AFFILIATES.  All rights reserved.
+
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from nemo_text_processing.text_normalization.en.graph_utils import GraphFst
-from nemo_text_processing.text_normalization.en.verbalizers.whitelist import WhiteListFst
-from nemo_text_processing.text_normalization.ru.verbalizers.cardinal import CardinalFst
-from nemo_text_processing.text_normalization.ru.verbalizers.date import DateFst
-from nemo_text_processing.text_normalization.ru.verbalizers.decimal import DecimalFst
-from nemo_text_processing.text_normalization.ru.verbalizers.electronic import ElectronicFst
-from nemo_text_processing.text_normalization.ru.verbalizers.measure import MeasureFst
-from nemo_text_processing.text_normalization.ru.verbalizers.money import MoneyFst
-from nemo_text_processing.text_normalization.ru.verbalizers.ordinal import OrdinalFst
-from nemo_text_processing.text_normalization.ru.verbalizers.telephone import TelephoneFst
-from nemo_text_processing.text_normalization.ru.verbalizers.time import TimeFst
+from nemo_text_processing.inverse_text_normalization.ar.verbalizers.cardinal import CardinalFst
+from nemo_text_processing.inverse_text_normalization.ar.verbalizers.decimal import DecimalFst
+from nemo_text_processing.inverse_text_normalization.ar.verbalizers.fraction import FractionFst
+from nemo_text_processing.inverse_text_normalization.ar.verbalizers.measure import MeasureFst
+from nemo_text_processing.inverse_text_normalization.ar.verbalizers.money import MoneyFst
+from nemo_text_processing.text_normalization.ar.graph_utils import GraphFst
 
 
 class VerbalizeFst(GraphFst):
     """
     Composes other verbalizer grammars.
     For deployment, this grammar will be compiled and exported to OpenFst Finite State Archive (FAR) File.
     More details to deployment at NeMo/tools/text_processing_deployment.
-
-    Args:
-        deterministic: if True will provide a single transduction option,
-            for False multiple options (used for audio-based normalization)
     """
 
-    def __init__(self, deterministic: bool = True):
-        super().__init__(name="verbalize", kind="verbalize", deterministic=deterministic)
+    def __init__(self):
+        super().__init__(name="verbalize", kind="verbalize")
         cardinal = CardinalFst()
         cardinal_graph = cardinal.fst
-        ordinal_graph = OrdinalFst().fst
         decimal = DecimalFst()
         decimal_graph = decimal.fst
-        date = DateFst()
-        date_graph = date.fst
-        measure = MeasureFst()
+        fraction = FractionFst()
+        fraction_graph = fraction.fst
+        money = MoneyFst(decimal, deterministic=True)
+        money_graph = money.fst
+        measure = MeasureFst(decimal=decimal, cardinal=cardinal, deterministic=True)
         measure_graph = measure.fst
-        electronic = ElectronicFst()
-        electronic_graph = electronic.fst
-        whitelist_graph = WhiteListFst().fst
-        money_graph = MoneyFst().fst
-        telephone_graph = TelephoneFst().fst
-        time_graph = TimeFst().fst
-
-        graph = (
-            measure_graph
-            | cardinal_graph
-            | decimal_graph
-            | ordinal_graph
-            | date_graph
-            | electronic_graph
-            | money_graph
-            | whitelist_graph
-            | telephone_graph
-            | time_graph
-        )
+        graph = cardinal_graph | decimal_graph | fraction_graph | money_graph | measure_graph
         self.fst = graph
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ru/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/run_evaluate.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/run_evaluate.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/ar/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/es/data/telephone/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/dates/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/electronic/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/unit.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/measure/unit_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_major.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_plural.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_minor_singular.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/money/currency_plurals.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/fractions/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/numbers/millions.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/ordinals/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/inflection/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/roman/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/telephone/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/data/whitelist.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/data/whitelist.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/graph_utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/abbreviation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/cardinal.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 
         # spoken this way, so useful for e2e ASR
         alt_ties = ties @ pynini.cdrewrite(ties_alt_endings, "", "[EOS]", NEMO_SIGMA)
         if not deterministic:
             ties |= pynutil.add_weight(alt_ties, -0.001)
             ties |= pynutil.add_weight(pynini.cross("4", "förtio"), -0.001)
             ties |= pynutil.add_weight(pynini.cross("4", "förti"), -0.001)
+            ties |= pynutil.add_weight(pynini.cross("2", "tju"), -0.001)
 
         # Any double digit
         graph_tens = teen
         graph_ties = ties
         if deterministic:
             graph_tens |= graph_ties + (pynutil.delete('0') | graph_digit)
         else:
@@ -324,14 +325,16 @@
             self.three_digits_read |= pynutil.add_weight(
                 ((NEMO_DIGIT - "0") + NEMO_DIGIT) @ graph_tens + insert_space + digit, -0.001
             )
             self.three_digits_read |= pynutil.add_weight(
                 digit + insert_space + ((NEMO_DIGIT - "0") + NEMO_DIGIT) @ graph_tens, -0.001
             )
             self.two_digits_read |= pynutil.add_weight(digit + insert_space + digit, -0.001)
+            self.any_read_digit |= self.two_digits_read
+            self.any_read_digit |= self.three_digits_read
 
         self.graph |= zero
 
         self.graph_unfiltered = self.graph
         self.graph = filter_punctuation(self.graph).optimize()
         self.graph_en = self.graph @ pynini.cdrewrite(ett_to_en, "", "[EOS]", NEMO_SIGMA)
         self.graph_no_one = (pynini.project(self.graph, "input") - "1") @ self.graph
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/decimal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/decimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     include_abbr: bool,
 ) -> 'pynini.FstLike':
     """
     Returns FST that transforms either a cardinal or decimal followed by a quantity into a numeral,
     e.g. 1 miljon -> integer_part: "en" quantity: "miljon"
     e.g. 1,5 miljoner -> integer_part: "en" fractional_part: "fem" quantity: "miljoner"
 
-    Args: 
+    Args:
         decimal: decimal FST
         cardinal_up_to_hundred: cardinal FST
     """
     quantities_pl = quantities + "er"
     # This is odd, but it's so we can accept miljard for miljarder
     quantities_pl |= quantities + pynutil.insert("er")
 
@@ -108,15 +108,15 @@
         + pynutil.insert("\"")
     )
     return res
 
 
 class DecimalFst(GraphFst):
     """
-    Finite state transducer for classifying decimal, e.g. 
+    Finite state transducer for classifying decimal, e.g.
         -12,5006 biljon -> decimal { negative: "true" integer_part: "tolv"  fractional_part: "fem noll noll sex" quantity: "biljon" }
         1 biljon -> decimal { integer_part: "en" quantity: "biljon" }
 
     cardinal: CardinalFst
     """
 
     def __init__(self, cardinal: GraphFst, deterministic: bool):
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from nemo_text_processing.text_normalization.sv.graph_utils import SV_ALPHA, TO_LOWER
 from nemo_text_processing.text_normalization.sv.utils import get_abs_path
 from pynini.lib import pynutil
 
 
 class MeasureFst(GraphFst):
     """
-    Finite state transducer for classifying measure, suppletive aware, e.g. 
+    Finite state transducer for classifying measure, suppletive aware, e.g.
         -12kg -> measure { negative: "true" cardinal { integer: "tolv" } units: "kilogram" }
         1kg -> measure { cardinal { integer: "ett" } units: "kilogram" }
         ,5kg -> measure { decimal { fractional_part: "fem" } units: "kilogram" }
 
     Args:
         cardinal: CardinalFst
         decimal: DecimalFst
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/money.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 maj_singular = pynini.string_file((get_abs_path("data/money/currency_major.tsv")))
 maj_singular_nt = pynini.string_file((get_abs_path("data/money/currency_major_nt.tsv")))
 maj_plural = pynini.string_file((get_abs_path("data/money/currency_plurals.tsv")))
 
 
 class MoneyFst(GraphFst):
     """
-    Finite state transducer for classifying money, suppletive aware, e.g. 
+    Finite state transducer for classifying money, suppletive aware, e.g.
         $12,05 -> money { integer_part: "tolv" currency_maj: "dollar" fractional_part: "fem" currency_min: "cent" preserve_order: true }
         $12,0500 -> money { integer_part: "tolv" currency_maj: "dollar" fractional_part: "fem" currency_min: "cent" preserve_order: true }
         $1 -> money { currency_maj: "dollar" integer_part: "en" }
         $1,00 -> money { currency_maj: "dollar" integer_part: "en" }
         $0,05 -> money { fractional_part: "fem"  currency_min: "cent" preserve_order: true }
         $1 miljon -> money { currency_maj: "dollar" integer_part: "en" quantity: "miljon" }
         $1,2 miljon -> money { currency_maj: "dollar" integer_part: "en"  fractional_part: "två" quantity: "miljon" }
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/taggers/telephone.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,132 +14,133 @@
 # limitations under the License.
 
 import pynini
 from nemo_text_processing.text_normalization.en.graph_utils import (
     NEMO_SPACE,
     GraphFst,
     delete_extra_space,
-    delete_space,
     insert_space,
 )
-from nemo_text_processing.text_normalization.sv.graph_utils import ensure_space
-from nemo_text_processing.text_normalization.sv.taggers.cardinal import CardinalFst
-from nemo_text_processing.text_normalization.sv.utils import get_abs_path
+from nemo_text_processing.text_normalization.hu.taggers.cardinal import CardinalFst
+from nemo_text_processing.text_normalization.hu.utils import get_abs_path
 from pynini.lib import pynutil
 
 
 class TelephoneFst(GraphFst):
     """
-    tfn. 08-789 52 25
+    tel: + (36) 1 441-4000
     Finite state transducer for classifying telephone numbers, e.g.
-        123-123-5678 -> { number_part: "ett två tre ett två tre fyra sex sju åtta" }.
+        + (36) 1 441-4000 -> { number_part: "plusz harminchat egy négyszáznegyvenegy négyezer" }.
+
+    Hungarian numbers are written in the following formats:
+        06 1 XXX XXXX
+        06 AA XXX-XXX
+        06 AA XXX-XXXX (mobile phones)
 
-    Swedish numbers are written in the following formats:
-        0X-XXX XXX XX
-        0X-XXX XX XX
-        0X-XX XX XX
-        0XX-XXX XX XX
-        0XX-XX XX XX
-        0XX-XXX XX
-        0XXX-XX XX XX
-        0XXX-XXX XX
-    
     See:
-        https://en.wikipedia.org/wiki/National_conventions_for_writing_telephone_numbers#Sweden
-        https://codegolf.stackexchange.com/questions/195787/format-a-swedish-phone-number
+        https://en.wikipedia.org/wiki/Telephone_numbers_in_Hungary
 
     Args:
 		deterministic: if True will provide a single transduction option,
 			for False multiple transduction are generated (used for audio-based normalization)
     """
 
     def __init__(self, deterministic: bool = True):
         super().__init__(name="telephone", kind="classify", deterministic=deterministic)
         cardinal = CardinalFst(deterministic)
-        add_separator = pynutil.insert(", ")
-        zero_space = cardinal.zero_space
+        area_codes = pynini.string_file(get_abs_path("data/telephone/area_codes.tsv")) @ cardinal.graph
+        self.area_codes = area_codes
+        country_codes = pynini.string_file(get_abs_path("data/telephone/country_codes.tsv")) @ cardinal.graph
+        self.country_codes = country_codes.optimize()
+
         digit = cardinal.digit
         two_digits = cardinal.two_digits_read
         three_digits = cardinal.three_digits_read
-        two_or_three_digits = (two_digits | three_digits).optimize()
-        one_two_or_three_digits = (digit | two_or_three_digits).optimize()
-        zero_after_country_code = pynini.union(pynini.cross("(0)", "noll "), zero_space)
-        bracketed = pynutil.delete("(") + one_two_or_three_digits + pynutil.delete(")")
+        four_digits = cardinal.four_digits_read
+        up_to_three_digits = digit | two_digits | three_digits
+        up_to_four_digits = up_to_three_digits | four_digits
+
+        separators = pynini.union(NEMO_SPACE, pynini.cross("-", " "))
+        area_separators = pynini.union(separators, pynini.cross("/", " "))
 
-        zero = pynini.cross("0", "noll")
+        zero = pynini.cross("0", "nulla")
         digit |= zero
 
         special_numbers = pynini.string_file(get_abs_path("data/telephone/special_numbers.tsv"))
+        special_numbers @= cardinal.three_digits_read
 
+        passable = pynini.union(":", ": ", " ")
+        prompt_pass = pynini.closure(pynutil.delete(passable) + insert_space, 0, 1)
         telephone_abbr = pynini.string_file(get_abs_path("data/telephone/telephone_abbr.tsv"))
+        telephone_abbr = telephone_abbr + prompt_pass
         telephone_prompt = pynini.string_file(get_abs_path("data/telephone/telephone_prompt.tsv"))
-        prompt = pynutil.insert("prompt: \"") + telephone_prompt + pynutil.insert("\"")
-        prompt |= pynutil.insert("prompt: \"") + telephone_abbr + pynutil.insert("\"")
-        prompt |= pynutil.insert("prompt: \"") + telephone_prompt + NEMO_SPACE + telephone_abbr + pynutil.insert("\"")
-
-        country_code = pynini.closure(pynini.cross("+", "plus "), 0, 1) + one_two_or_three_digits
-        country_code = pynutil.insert("country_code: \"") + country_code + pynutil.insert("\"")
-
-        opt_dash = pynini.closure(pynutil.delete("-"), 0, 1)
-        area_part = zero_after_country_code + one_two_or_three_digits + opt_dash + add_separator
-        area_part |= bracketed + add_separator
+        prompt_as_code = pynutil.insert("country_code: \"") + telephone_prompt + pynutil.insert("\"")
+        prompt_as_code |= pynutil.insert("country_code: \"") + telephone_abbr + pynutil.insert("\"")
+        prompt_as_code |= (
+            pynutil.insert("country_code: \"") + telephone_prompt + NEMO_SPACE + telephone_abbr + pynutil.insert("\"")
+        )
+        prompt_inner = telephone_prompt | telephone_abbr
+        prompt_inner |= telephone_prompt + NEMO_SPACE + telephone_abbr
+
+        plus = pynini.cross("+", "plusz ")
+        plus |= pynini.cross("00", "nulla nulla ")
+        plus = plus + pynini.closure(pynutil.delete(" "), 0, 1)
+
+        country = pynini.closure(pynutil.delete("("), 0, 1) + country_codes + pynini.closure(pynutil.delete(")"), 0, 1)
+        country = plus + pynini.closure(pynutil.delete(" "), 0, 1) + country
+        country_code = pynutil.insert("country_code: \"") + country + pynutil.insert("\"")
+        country_code |= prompt_as_code
+        country_code |= pynutil.insert("country_code: \"") + prompt_inner + NEMO_SPACE + country + pynutil.insert("\"")
+
+        trunk = pynini.cross("06", "nulla hat")
+        trunk |= pynutil.delete("(") + trunk + pynutil.delete(")")
+
+        area_part = area_codes + area_separators
 
         base_number_part = pynini.union(
-            three_digits + NEMO_SPACE + three_digits + NEMO_SPACE + two_digits,
-            three_digits + NEMO_SPACE + two_digits + NEMO_SPACE + two_digits,
-            three_digits + NEMO_SPACE + two_digits + insert_space + two_digits,
-            two_digits + NEMO_SPACE + two_digits + NEMO_SPACE + two_digits,
-            two_digits + NEMO_SPACE + two_digits + insert_space + two_digits,
-            three_digits + NEMO_SPACE + two_digits,
+            three_digits + separators + three_digits,
+            three_digits + separators + two_digits + separators + two_digits,
+            three_digits + separators + four_digits,
+            two_digits + separators + four_digits,
+            four_digits + separators + three_digits,
+            two_digits + separators + two_digits + separators + three_digits,
         )
-        number_part = area_part + delete_space + base_number_part
+        number_part = area_part + base_number_part
 
         self.number_graph = number_part
-        number_part = pynutil.insert("number_part: \"") + number_part + pynutil.insert("\"")
-        extension = pynutil.insert("extension: \"") + one_two_or_three_digits + pynutil.insert("\"")
-        extension = pynini.closure(insert_space + extension, 0, 1)
-        ext_prompt = NEMO_SPACE + pynutil.delete(pynini.union("ankn", "ankn.", "anknytning")) + ensure_space
-        passable = pynini.union(":", ": ", " ")
-        prompt_pass = pynutil.delete(passable) + insert_space
+        number_part = pynutil.insert("number_part: \"") + self.number_graph + pynutil.insert("\"")
+        trunk_number_part = (
+            pynutil.insert("number_part: \"") + trunk + separators + self.number_graph + pynutil.insert("\"")
+        )
+        mellek = NEMO_SPACE + pynutil.delete("mellék")
+        extension = pynutil.insert("extension: \"") + up_to_four_digits + pynutil.insert("\"")
+        extension = pynini.closure(area_separators + extension + mellek, 0, 1)
 
         special_numbers = pynutil.insert("number_part: \"") + special_numbers + pynutil.insert("\"")
-        prompt = prompt + prompt_pass
         graph = pynini.union(
-            country_code + ensure_space + number_part,
-            country_code + ensure_space + number_part + ext_prompt + extension,
-            number_part + ext_prompt + extension,
-            prompt + number_part,
-            prompt + special_numbers,
-            prompt + country_code + number_part,
-            prompt + country_code + number_part + ext_prompt + extension,
-            prompt + number_part + ext_prompt + extension,
+            country_code + separators + number_part,
+            country_code + separators + number_part + extension,
+            number_part + extension,
+            trunk_number_part,
+            trunk_number_part + extension,
+            country_code + number_part,
+            country_code + trunk_number_part,
+            country_code + trunk_number_part + extension,
+            country_code + special_numbers,
+            country_code + number_part + extension,
         )
         self.tel_graph = graph.optimize()
 
         # ip
         ip_prompts = pynini.string_file(get_abs_path("data/telephone/ip_prompt.tsv"))
-        ip_graph = one_two_or_three_digits + (pynini.cross(".", " punkt ") + one_two_or_three_digits) ** 3
+        ip_graph = up_to_three_digits + (pynini.cross(".", " pont ") + up_to_three_digits) ** 3
         graph |= (
             pynini.closure(
                 pynutil.insert("country_code: \"") + ip_prompts + pynutil.insert("\"") + delete_extra_space, 0, 1
             )
             + pynutil.insert("number_part: \"")
             + ip_graph.optimize()
             + pynutil.insert("\"")
         )
-        # ssn
-        ssn_prompts = pynini.string_file(get_abs_path("data/telephone/ssn_prompt.tsv"))
-        four_digit_part = digit + (pynutil.insert(" ") + digit) ** 3
-        ssn_separator = pynini.cross("-", ", ")
-        ssn_graph = three_digits + ssn_separator + two_digits + ssn_separator + four_digit_part
-
-        graph |= (
-            pynini.closure(
-                pynutil.insert("country_code: \"") + ssn_prompts + pynutil.insert("\"") + delete_extra_space, 0, 1
-            )
-            + pynutil.insert("number_part: \"")
-            + ssn_graph.optimize()
-            + pynutil.insert("\"")
-        )
 
         final_graph = self.add_tokens(graph)
         self.fst = final_graph.optimize()
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         2.30 e.m. -> time { hours: "två" minutes: "trettio" suffix: "eftermiddag" }
         02.30 e.m. -> time { hours: "två" minutes: "trettio" suffix: "eftermiddag" }
         2.00 e.m. -> time { hours: "två" suffix: "eftermiddag" }
         kl. 2 e.m. -> time { hours: "två" suffix: "eftermiddag" }
         02:00 -> time { hours: "två" }
         2:00 -> time { hours: "två" }
         10:00:05 e.m. -> time { hours: "tio" minutes: "noll" seconds: "fem" suffix: "eftermiddag" }
-    
+
     Args:
         cardinal: CardinalFst
         deterministic: if True will provide a single transduction option,
             for False multiple transduction are generated (used for audio-based normalization)
     """
 
     def __init__(self, cardinal: GraphFst, deterministic: bool = True):
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 from nemo_text_processing.text_normalization.sv.taggers.word import WordFst
 from pynini.lib import pynutil
 
 
 class ClassifyFst(GraphFst):
     """
     Final class that composes all other classification grammars. This class can process an entire sentence including punctuation.
-    For deployment, this grammar will be compiled and exported to OpenFst Finite State Archive (FAR) File. 
+    For deployment, this grammar will be compiled and exported to OpenFst Finite State Archive (FAR) File.
     More details to deployment at NeMo/tools/text_processing_deployment.
-    
+
     Args:
         input_case: accepting either "lower_cased" or "cased" input.
         deterministic: if True will provide a single transduction option,
             for False multiple options (used for audio-based normalization)
         cache_dir: path to a dir with .far grammar file. Set to None to avoid using cache.
         overwrite_cache: set to True to overwrite .far files
         whitelist: path to a file with whitelist replacements
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/tokenize_and_classify_with_audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 from nemo_text_processing.text_normalization.sv.verbalizers.time import TimeFst as vTimeFst
 from pynini.lib import pynutil
 
 
 class ClassifyFst(GraphFst):
     """
     Final class that composes all other classification grammars. This class can process an entire sentence including punctuation.
-    For deployment, this grammar will be compiled and exported to OpenFst Finate State Archive (FAR) File. 
+    For deployment, this grammar will be compiled and exported to OpenFst Finate State Archive (FAR) File.
     More details to deployment at NeMo/tools/text_processing_deployment.
-    
+
     Args:
         input_case: accepting either "lower_cased" or "cased" input.
         deterministic: if True will provide a single transduction option,
             for False multiple options (used for audio-based normalization)
         cache_dir: path to a dir with .far grammar file. Set to None to avoid using cache.
         overwrite_cache: set to True to overwrite .far files
         whitelist: path to a file with whitelist replacements
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/taggers/word.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/taggers/word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def get_abs_path(rel_path):
     """
     Get absolute path
 
     Args:
         rel_path: relative path to this file
-        
+
     Returns absolute path
     """
     return os.path.dirname(os.path.abspath(__file__)) + '/' + rel_path
 
 
 def load_labels(abs_path):
     """
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/hu/data/ordinals/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/decimals.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class MeasureFst(GraphFst):
     """
     Finite state transducer for verbalizing measure, e.g.
         measure { negative: "true" cardinal { integer: "twelve" } units: "kilograms" } -> minus twelve kilograms
         measure { decimal { integer_part: "twelve" fractional_part: "five" } units: "kilograms" } -> twelve point five kilograms
         tokens { measure { units: "covid" decimal { integer_part: "nineteen"  fractional_part: "five" }  } } -> covid nineteen point five
-    
+
     Args:
         decimal: DecimalFst
         cardinal: CardinalFst
         fraction: FractionFst
         deterministic: if True will provide a single transduction option,
             for False multiple transduction are generated (used for audio-based normalization)
     """
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/telephone.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,14 @@
     def __init__(self, deterministic: bool = True):
         super().__init__(name="telephone", kind="verbalize", deterministic=deterministic)
 
         country_code = pynutil.delete("country_code: \"") + pynini.closure(NEMO_NOT_QUOTE, 1) + pynutil.delete("\"")
 
         optional_country_code = pynini.closure(country_code + delete_space + insert_space, 0, 1,)
 
-        prompt_part = (
-            pynutil.delete("prompt: \"")
-            + pynini.closure(NEMO_NOT_QUOTE, 1)
-            + pynini.closure(pynutil.add_weight(pynutil.delete(" "), -0.0001), 0, 1)
-            + pynutil.delete("\"")
-        ) + NEMO_SPACE
-
         number_part = (
             pynutil.delete("number_part: \"")
             + pynini.closure(NEMO_NOT_QUOTE, 1)
             + pynini.closure(pynutil.add_weight(pynutil.delete(" "), -0.0001), 0, 1)
             + pynutil.delete("\"")
         )
 
@@ -61,13 +54,10 @@
             + pynini.cross("extension: \"", "anknytning ")
             + pynini.closure(NEMO_NOT_QUOTE, 1)
             + pynutil.delete("\""),
             0,
             1,
         )
 
-        graph = pynini.union(
-            prompt_part + optional_country_code + number_part + optional_extension,
-            optional_country_code + number_part + optional_extension,
-        )
+        graph = pynini.union(optional_country_code + number_part + optional_extension)
         delete_tokens = self.delete_tokens(graph)
         self.fst = delete_tokens.optimize()
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/sv/verbalizers/verbalize_final.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         if cache_dir is not None and cache_dir != "None":
             os.makedirs(cache_dir, exist_ok=True)
             far_file = os.path.join(cache_dir, f"sv_tn_{deterministic}_deterministic_verbalizer.far")
         if not overwrite_cache and far_file and os.path.exists(far_file):
             self.fst = pynini.Far(far_file, mode="r")["verbalize"]
             logging.info(f'VerbalizeFinalFst graph was restored from {far_file}.')
         else:
-
             verbalize = VerbalizeFst(deterministic=deterministic).fst
             word = WordFst(deterministic=deterministic).fst
             types = verbalize | word
             graph = (
                 pynutil.delete("tokens")
                 + delete_space
                 + pynutil.delete("{")
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/token_parser.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/token_parser.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/utils_audio_based.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/utils_audio_based.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/charset_national_standard_2013_8105.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/char/fullwidth_to_halfwidth.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/date/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/date/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/denylist/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/erhua/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/math/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/math/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/measure/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/measure/units_en.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/measure/units_zh.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/measure/units_zh.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/money/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/money/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/money/currency_code.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/money/currency_code.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/money/currency_symbol.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/money/currency_symbol.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/number/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/number/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/time/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/time/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/whitelist/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/whitelist/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/data/whitelist/default.tsv` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/data/whitelist/default.tsv`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/graph_utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/graph_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+import logging
 import os
 import string
 from pathlib import Path
 from typing import Dict
 
 import pynini
 from pynini import Far
@@ -52,15 +54,15 @@
         file_name: exported file name
         graphs: Mapping of a rule name and Pynini WFST graph to be exported
     """
     exporter = export.Exporter(file_name)
     for rule, graph in graphs.items():
         exporter[rule] = graph.optimize()
     exporter.close()
-    print(f'Created {file_name}')
+    logging.info(f'Created {file_name}')
 
 
 class GraphFst:
     """
     Base class for all grammar fsts.
 
     Args:
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/char.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/char.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/math_symbol.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/math_symbol.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/preprocessor.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/tokenize_and_classify.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/taggers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/taggers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/utils.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/utils.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/char.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/char.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/date.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/math_symbol.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/math_symbol.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/measure.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/money.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/postprocessor.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/time.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/verbalize_final.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/PKG-INFO` & `nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo-text-processing
-Version: 0.1.7rc0
+Version: 0.1.8rc0
 Summary: NeMo text processing for ASR and TTS
 Home-page: https://github.com/nvidia/nemo-text-processing
 Download-URL: https://github.com/NVIDIA/NeMo-text-processing/releases
 Author: NVIDIA
 Author-email: nemo-toolkit@nvidia.com
 Maintainer: NVIDIA
 Maintainer-email: nemo-toolkit@nvidia.com
```

### Comparing `nemo_text_processing-0.1.7rc0/nemo_text_processing.egg-info/SOURCES.txt` & `nemo_text_processing-0.1.8rc0/nemo_text_processing.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,36 +9,40 @@
 nemo_text_processing.egg-info/SOURCES.txt
 nemo_text_processing.egg-info/dependency_links.txt
 nemo_text_processing.egg-info/not-zip-safe
 nemo_text_processing.egg-info/requires.txt
 nemo_text_processing.egg-info/top_level.txt
 nemo_text_processing/fst_alignment/__init__.py
 nemo_text_processing/fst_alignment/alignment.py
+nemo_text_processing/g2p/__init__.py
+nemo_text_processing/g2p/data/__init__.py
 nemo_text_processing/hybrid/__init__.py
 nemo_text_processing/hybrid/mlm_scorer.py
 nemo_text_processing/hybrid/model_utils.py
 nemo_text_processing/hybrid/utils.py
 nemo_text_processing/hybrid/wfst_lm_rescoring.py
 nemo_text_processing/inverse_text_normalization/__init__.py
 nemo_text_processing/inverse_text_normalization/inverse_normalize.py
 nemo_text_processing/inverse_text_normalization/run_evaluate.py
 nemo_text_processing/inverse_text_normalization/ar/__init__.py
 nemo_text_processing/inverse_text_normalization/ar/utils.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/__init__.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/cardinal.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/decimal.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/fraction.py
+nemo_text_processing/inverse_text_normalization/ar/taggers/measure.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/money.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/punctuation.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/tokenize_and_classify.py
 nemo_text_processing/inverse_text_normalization/ar/taggers/word.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/__init__.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/cardinal.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/decimal.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/fraction.py
+nemo_text_processing/inverse_text_normalization/ar/verbalizers/measure.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/money.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/verbalize_final.py
 nemo_text_processing/inverse_text_normalization/ar/verbalizers/word.py
 nemo_text_processing/inverse_text_normalization/de/__init__.py
 nemo_text_processing/inverse_text_normalization/de/taggers/__init__.py
 nemo_text_processing/inverse_text_normalization/de/taggers/cardinal.py
@@ -436,14 +440,16 @@
 nemo_text_processing/text_normalization/run_evaluate.py
 nemo_text_processing/text_normalization/token_parser.py
 nemo_text_processing/text_normalization/utils_audio_based.py
 nemo_text_processing/text_normalization/ar/__init__.py
 nemo_text_processing/text_normalization/ar/graph_utils.py
 nemo_text_processing/text_normalization/ar/utils.py
 nemo_text_processing/text_normalization/ar/data/__init__.py
+nemo_text_processing/text_normalization/ar/data/measure/__init__.py
+nemo_text_processing/text_normalization/ar/data/measure/measurements.tsv
 nemo_text_processing/text_normalization/ar/data/money/__init__.py
 nemo_text_processing/text_normalization/ar/data/money/currency_major.tsv
 nemo_text_processing/text_normalization/ar/data/money/currency_minor_plural.tsv
 nemo_text_processing/text_normalization/ar/data/money/currency_minor_singular.tsv
 nemo_text_processing/text_normalization/ar/data/money/local_currency.tsv
 nemo_text_processing/text_normalization/ar/data/number/__init__.py
 nemo_text_processing/text_normalization/ar/data/number/digit.tsv
@@ -458,21 +464,23 @@
 nemo_text_processing/text_normalization/ar/data/number/teens.tsv
 nemo_text_processing/text_normalization/ar/data/number/tens.tsv
 nemo_text_processing/text_normalization/ar/data/number/zero.tsv
 nemo_text_processing/text_normalization/ar/taggers/__init__.py
 nemo_text_processing/text_normalization/ar/taggers/cardinal.py
 nemo_text_processing/text_normalization/ar/taggers/decimal.py
 nemo_text_processing/text_normalization/ar/taggers/fraction.py
+nemo_text_processing/text_normalization/ar/taggers/measure.py
 nemo_text_processing/text_normalization/ar/taggers/money.py
 nemo_text_processing/text_normalization/ar/taggers/tokenize_and_classify.py
 nemo_text_processing/text_normalization/ar/taggers/word.py
 nemo_text_processing/text_normalization/ar/verbalizers/__init__.py
 nemo_text_processing/text_normalization/ar/verbalizers/cardinal.py
 nemo_text_processing/text_normalization/ar/verbalizers/decimal.py
 nemo_text_processing/text_normalization/ar/verbalizers/fraction.py
+nemo_text_processing/text_normalization/ar/verbalizers/measure.py
 nemo_text_processing/text_normalization/ar/verbalizers/money.py
 nemo_text_processing/text_normalization/ar/verbalizers/verbalize.py
 nemo_text_processing/text_normalization/ar/verbalizers/verbalize_final.py
 nemo_text_processing/text_normalization/ar/verbalizers/word.py
 nemo_text_processing/text_normalization/de/__init__.py
 nemo_text_processing/text_normalization/de/utils.py
 nemo_text_processing/text_normalization/de/data/__init__.py
@@ -729,14 +737,95 @@
 nemo_text_processing/text_normalization/es/verbalizers/measure.py
 nemo_text_processing/text_normalization/es/verbalizers/money.py
 nemo_text_processing/text_normalization/es/verbalizers/ordinal.py
 nemo_text_processing/text_normalization/es/verbalizers/telephone.py
 nemo_text_processing/text_normalization/es/verbalizers/time.py
 nemo_text_processing/text_normalization/es/verbalizers/verbalize.py
 nemo_text_processing/text_normalization/es/verbalizers/verbalize_final.py
+nemo_text_processing/text_normalization/hu/__init__.py
+nemo_text_processing/text_normalization/hu/graph_utils.py
+nemo_text_processing/text_normalization/hu/utils.py
+nemo_text_processing/text_normalization/hu/data/__init__.py
+nemo_text_processing/text_normalization/hu/data/math_operations.tsv
+nemo_text_processing/text_normalization/hu/data/whitelist.tsv
+nemo_text_processing/text_normalization/hu/data/whitelist_inflect.tsv
+nemo_text_processing/text_normalization/hu/data/whitelist_inflect_sg.tsv
+nemo_text_processing/text_normalization/hu/data/dates/__init__.py
+nemo_text_processing/text_normalization/hu/data/dates/days.tsv
+nemo_text_processing/text_normalization/hu/data/dates/days_to_numbers.tsv
+nemo_text_processing/text_normalization/hu/data/dates/month_abbr.tsv
+nemo_text_processing/text_normalization/hu/data/dates/months.tsv
+nemo_text_processing/text_normalization/hu/data/dates/months_roman.tsv
+nemo_text_processing/text_normalization/hu/data/electronic/__init__.py
+nemo_text_processing/text_normalization/hu/data/electronic/domain.tsv
+nemo_text_processing/text_normalization/hu/data/electronic/server_name.tsv
+nemo_text_processing/text_normalization/hu/data/electronic/symbols.tsv
+nemo_text_processing/text_normalization/hu/data/fractions/__init__.py
+nemo_text_processing/text_normalization/hu/data/fractions/fraction_symbols.tsv
+nemo_text_processing/text_normalization/hu/data/inflection/__init__.py
+nemo_text_processing/text_normalization/hu/data/inflection/endings.tsv
+nemo_text_processing/text_normalization/hu/data/inflection/plural_endings.tsv
+nemo_text_processing/text_normalization/hu/data/inflection/word_endings.tsv
+nemo_text_processing/text_normalization/hu/data/measures/__init__.py
+nemo_text_processing/text_normalization/hu/data/measures/greek_lower.tsv
+nemo_text_processing/text_normalization/hu/data/measures/greek_upper.tsv
+nemo_text_processing/text_normalization/hu/data/measures/measurements.tsv
+nemo_text_processing/text_normalization/hu/data/money/__init__.py
+nemo_text_processing/text_normalization/hu/data/money/alphabet.tsv
+nemo_text_processing/text_normalization/hu/data/money/currency.tsv
+nemo_text_processing/text_normalization/hu/data/money/currency_minor.tsv
+nemo_text_processing/text_normalization/hu/data/number/__init__.py
+nemo_text_processing/text_normalization/hu/data/number/digit.tsv
+nemo_text_processing/text_normalization/hu/data/number/digit_inline.tsv
+nemo_text_processing/text_normalization/hu/data/number/digit_nom.tsv
+nemo_text_processing/text_normalization/hu/data/number/quantities.tsv
+nemo_text_processing/text_normalization/hu/data/number/tens.tsv
+nemo_text_processing/text_normalization/hu/data/number/tens_inline.tsv
+nemo_text_processing/text_normalization/hu/data/number/zero.tsv
+nemo_text_processing/text_normalization/hu/data/ordinals/__init__.py
+nemo_text_processing/text_normalization/hu/data/ordinals/endings.tsv
+nemo_text_processing/text_normalization/hu/data/ordinals/exceptional.tsv
+nemo_text_processing/text_normalization/hu/data/ordinals/superessive_endings.tsv
+nemo_text_processing/text_normalization/hu/data/ordinals/superscript_digits.tsv
+nemo_text_processing/text_normalization/hu/data/telephone/__init__.py
+nemo_text_processing/text_normalization/hu/data/telephone/area_codes.tsv
+nemo_text_processing/text_normalization/hu/data/telephone/country_codes.tsv
+nemo_text_processing/text_normalization/hu/data/telephone/ip_prompt.tsv
+nemo_text_processing/text_normalization/hu/data/telephone/special_numbers.tsv
+nemo_text_processing/text_normalization/hu/data/telephone/telephone_abbr.tsv
+nemo_text_processing/text_normalization/hu/data/telephone/telephone_prompt.tsv
+nemo_text_processing/text_normalization/hu/data/time/__init__.py
+nemo_text_processing/text_normalization/hu/data/time/time_zone.tsv
+nemo_text_processing/text_normalization/hu/taggers/__init__.py
+nemo_text_processing/text_normalization/hu/taggers/cardinal.py
+nemo_text_processing/text_normalization/hu/taggers/date.py
+nemo_text_processing/text_normalization/hu/taggers/decimal.py
+nemo_text_processing/text_normalization/hu/taggers/electronic.py
+nemo_text_processing/text_normalization/hu/taggers/fraction.py
+nemo_text_processing/text_normalization/hu/taggers/measure.py
+nemo_text_processing/text_normalization/hu/taggers/money.py
+nemo_text_processing/text_normalization/hu/taggers/ordinal.py
+nemo_text_processing/text_normalization/hu/taggers/telephone.py
+nemo_text_processing/text_normalization/hu/taggers/time.py
+nemo_text_processing/text_normalization/hu/taggers/tokenize_and_classify.py
+nemo_text_processing/text_normalization/hu/taggers/whitelist.py
+nemo_text_processing/text_normalization/hu/taggers/word.py
+nemo_text_processing/text_normalization/hu/verbalizers/__init__.py
+nemo_text_processing/text_normalization/hu/verbalizers/cardinal.py
+nemo_text_processing/text_normalization/hu/verbalizers/date.py
+nemo_text_processing/text_normalization/hu/verbalizers/decimal.py
+nemo_text_processing/text_normalization/hu/verbalizers/electronic.py
+nemo_text_processing/text_normalization/hu/verbalizers/fraction.py
+nemo_text_processing/text_normalization/hu/verbalizers/measure.py
+nemo_text_processing/text_normalization/hu/verbalizers/money.py
+nemo_text_processing/text_normalization/hu/verbalizers/ordinal.py
+nemo_text_processing/text_normalization/hu/verbalizers/telephone.py
+nemo_text_processing/text_normalization/hu/verbalizers/time.py
+nemo_text_processing/text_normalization/hu/verbalizers/verbalize.py
+nemo_text_processing/text_normalization/hu/verbalizers/verbalize_final.py
 nemo_text_processing/text_normalization/ru/__init__.py
 nemo_text_processing/text_normalization/ru/alphabet.py
 nemo_text_processing/text_normalization/ru/utils.py
 nemo_text_processing/text_normalization/ru/data/__init__.py
 nemo_text_processing/text_normalization/ru/data/latin_to_cyrillic.tsv
 nemo_text_processing/text_normalization/ru/data/measurements.tsv
 nemo_text_processing/text_normalization/ru/data/whitelist.tsv
@@ -845,14 +934,15 @@
 nemo_text_processing/text_normalization/sv/data/ordinals/ties.tsv
 nemo_text_processing/text_normalization/sv/data/ordinals/zero.tsv
 nemo_text_processing/text_normalization/sv/data/roman/__init__.py
 nemo_text_processing/text_normalization/sv/data/roman/digit.tsv
 nemo_text_processing/text_normalization/sv/data/roman/hundreds.tsv
 nemo_text_processing/text_normalization/sv/data/roman/ties.tsv
 nemo_text_processing/text_normalization/sv/data/telephone/__init__.py
+nemo_text_processing/text_normalization/sv/data/telephone/country_codes.tsv
 nemo_text_processing/text_normalization/sv/data/telephone/ip_prompt.tsv
 nemo_text_processing/text_normalization/sv/data/telephone/special_numbers.tsv
 nemo_text_processing/text_normalization/sv/data/telephone/ssn_prompt.tsv
 nemo_text_processing/text_normalization/sv/data/telephone/telephone_abbr.tsv
 nemo_text_processing/text_normalization/sv/data/telephone/telephone_prompt.tsv
 nemo_text_processing/text_normalization/sv/data/time/__init__.py
 nemo_text_processing/text_normalization/sv/data/time/hour_to.tsv
@@ -955,14 +1045,21 @@
 nemo_text_processing/text_normalization/zh/verbalizers/whitelist.py
 requirements/requirements.txt
 requirements/requirements_test.txt
 tests/__init__.py
 tests/conftest.py
 tests/nemo_text_processing/__init__.py
 tests/nemo_text_processing/utils.py
+tests/nemo_text_processing/ar/__init__.py
+tests/nemo_text_processing/ar/test_cardinal.py
+tests/nemo_text_processing/ar/test_decimal.py
+tests/nemo_text_processing/ar/test_fraction.py
+tests/nemo_text_processing/ar/test_measure.py
+tests/nemo_text_processing/ar/test_money.py
+tests/nemo_text_processing/ar/test_whitelist.py
 tests/nemo_text_processing/de/__init__.py
 tests/nemo_text_processing/de/test_cardinal.py
 tests/nemo_text_processing/de/test_date.py
 tests/nemo_text_processing/de/test_decimal.py
 tests/nemo_text_processing/de/test_electronic.py
 tests/nemo_text_processing/de/test_fraction.py
 tests/nemo_text_processing/de/test_measure.py
@@ -1018,14 +1115,28 @@
 tests/nemo_text_processing/fr/test_measure.py
 tests/nemo_text_processing/fr/test_money.py
 tests/nemo_text_processing/fr/test_ordinal.py
 tests/nemo_text_processing/fr/test_telephone.py
 tests/nemo_text_processing/fr/test_time.py
 tests/nemo_text_processing/fr/test_whitelist.py
 tests/nemo_text_processing/fr/test_word.py
+tests/nemo_text_processing/hu/__init__.py
+tests/nemo_text_processing/hu/test_cardinal.py
+tests/nemo_text_processing/hu/test_date.py
+tests/nemo_text_processing/hu/test_decimal.py
+tests/nemo_text_processing/hu/test_electronic.py
+tests/nemo_text_processing/hu/test_fraction.py
+tests/nemo_text_processing/hu/test_measure.py
+tests/nemo_text_processing/hu/test_money.py
+tests/nemo_text_processing/hu/test_ordinal.py
+tests/nemo_text_processing/hu/test_telephone.py
+tests/nemo_text_processing/hu/test_time.py
+tests/nemo_text_processing/hu/test_whitelist.py
+tests/nemo_text_processing/hu/test_word.py
+tests/nemo_text_processing/hu/data_text_normalization/__init__.py
 tests/nemo_text_processing/pt/__init__.py
 tests/nemo_text_processing/pt/test_cardinal.py
 tests/nemo_text_processing/pt/test_date.py
 tests/nemo_text_processing/pt/test_decimal.py
 tests/nemo_text_processing/pt/test_electronic.py
 tests/nemo_text_processing/pt/test_measure.py
 tests/nemo_text_processing/pt/test_money.py
@@ -1034,26 +1145,14 @@
 tests/nemo_text_processing/pt/test_time.py
 tests/nemo_text_processing/pt/test_whitelist.py
 tests/nemo_text_processing/pt/test_word.py
 tests/nemo_text_processing/ru/__init__.py
 tests/nemo_text_processing/ru/test_ru_inverse_normalization.py
 tests/nemo_text_processing/ru/test_ru_normalization.py
 tests/nemo_text_processing/ru/data_text_normalization/__init__.py
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_cardinal.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_cardinal_normalize_with_audio.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_date.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_decimal.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_electronic.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_measure.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_money.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_ordinal.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_telephone.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_time.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_whitelist.txt
-tests/nemo_text_processing/ru/data_text_normalization/test_cases_word.txt
 tests/nemo_text_processing/sv/__init__.py
 tests/nemo_text_processing/sv/test_cardinal.py
 tests/nemo_text_processing/sv/test_date.py
 tests/nemo_text_processing/sv/test_decimal.py
 tests/nemo_text_processing/sv/test_electronic.py
 tests/nemo_text_processing/sv/test_fraction.py
 tests/nemo_text_processing/sv/test_measure.py
```

### Comparing `nemo_text_processing-0.1.7rc0/setup.cfg` & `nemo_text_processing-0.1.8rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/setup.py` & `nemo_text_processing-0.1.8rc0/setup.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/conftest.py` & `nemo_text_processing-0.1.8rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_cardinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_decimal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_electronic.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_fraction.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_normalization_with_audio.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_ordinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_telephone.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_whitelist.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/de/test_word.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/de/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_address.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_address.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_cardinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_decimal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_electronic.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_fraction.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_math.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_math.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_normalization_with_audio.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_ordinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_punctuation.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_punctuation.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_range.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_range.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_roman.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_roman.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_serial.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_serial.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_special_text.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_special_text.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_telephone.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_text_split.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_text_split.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_whitelist.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/en/test_word.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/en/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/__init__.py` & `nemo_text_processing-0.1.8rc0/nemo_text_processing/text_normalization/en/data/address/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_cardinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_decimal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_decimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,14 @@
     )
 
     @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_decimal.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
     def test_norm(self, test_input, expected):
         pred = self.normalizer.normalize(test_input, verbose=False)
-        assert pred == expected
+        assert pred in expected
 
         if self.normalizer_with_audio:
             pred_non_deterministic = self.normalizer_with_audio.normalize(
                 test_input, n_tagged=500, punct_post_process=False
             )
             assert expected in pred_non_deterministic
```

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_electronic.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_fraction.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
     )
 
     @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_measure.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
     def test_norm(self, test_input, expected):
         pred = self.normalizer.normalize(test_input, verbose=False)
-        assert pred == expected
+        assert pred in expected
 
         if self.normalizer_with_audio:
             pred_non_deterministic = self.normalizer_with_audio.normalize(
                 test_input, n_tagged=500, punct_post_process=False
             )
             assert expected in pred_non_deterministic
```

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_normalization_with_audio.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_ordinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,46 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 import pytest
 from nemo_text_processing.inverse_text_normalization.inverse_normalize import InverseNormalizer
 from nemo_text_processing.text_normalization.normalize import Normalizer
 from nemo_text_processing.text_normalization.normalize_with_audio import NormalizerWithAudio
 from parameterized import parameterized
 
 from ..utils import CACHE_DIR, RUN_AUDIO_BASED_TESTS, parse_test_case_file
 
 
-class TestOrdinal:
-    inverse_normalizer = InverseNormalizer(lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
+class TestTime:
+    inverse_normalizer_es = InverseNormalizer(lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
 
-    @parameterized.expand(parse_test_case_file('es/data_inverse_text_normalization/test_cases_ordinal.txt'))
+    @parameterized.expand(parse_test_case_file('es/data_inverse_text_normalization/test_cases_time.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
-    def test_denorm(self, test_input, expected):
-        pred = self.inverse_normalizer.inverse_normalize(test_input, verbose=False)
+    def test_denorm_es(self, test_input, expected):
+        pred = self.inverse_normalizer_es.inverse_normalize(test_input, verbose=False)
         assert pred == expected
 
     normalizer = Normalizer(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
+
     normalizer_with_audio = (
         NormalizerWithAudio(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
         if CACHE_DIR and RUN_AUDIO_BASED_TESTS
         else None
     )
 
-    @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_ordinal.txt'))
+    @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_time.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
     def test_norm(self, test_input, expected):
         pred = self.normalizer.normalize(test_input, verbose=False)
         assert pred == expected
 
         if self.normalizer_with_audio:
             pred_non_deterministic = self.normalizer_with_audio.normalize(
-                test_input, n_tagged=500, punct_post_process=False,
+                test_input, n_tagged=500, punct_post_process=False
             )
             assert expected in pred_non_deterministic
```

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_telephone.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_telephone.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,14 @@
     )
 
     @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_telephone.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
     def test_norm(self, test_input, expected):
         pred = self.normalizer.normalize(test_input, verbose=False)
-        assert pred == expected
+        assert pred in expected
 
         if self.normalizer_with_audio:
             pred_non_deterministic = self.normalizer_with_audio.normalize(
                 test_input, n_tagged=30, punct_post_process=False
             )
             assert expected in pred_non_deterministic
```

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_word.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,37 +17,36 @@
 from nemo_text_processing.text_normalization.normalize import Normalizer
 from nemo_text_processing.text_normalization.normalize_with_audio import NormalizerWithAudio
 from parameterized import parameterized
 
 from ..utils import CACHE_DIR, RUN_AUDIO_BASED_TESTS, parse_test_case_file
 
 
-class TestTime:
+class TestWord:
     inverse_normalizer_es = InverseNormalizer(lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
 
-    @parameterized.expand(parse_test_case_file('es/data_inverse_text_normalization/test_cases_time.txt'))
+    @parameterized.expand(parse_test_case_file('es/data_inverse_text_normalization/test_cases_word.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
     def test_denorm_es(self, test_input, expected):
         pred = self.inverse_normalizer_es.inverse_normalize(test_input, verbose=False)
         assert pred == expected
 
-    normalizer = Normalizer(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
-
-    normalizer_with_audio = (
+    normalizer_es = Normalizer(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
+    normalizer_with_audio_es = (
         NormalizerWithAudio(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
         if CACHE_DIR and RUN_AUDIO_BASED_TESTS
         else None
     )
 
-    @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_time.txt'))
+    @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_word.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
     def test_norm(self, test_input, expected):
-        pred = self.normalizer.normalize(test_input, verbose=False)
-        assert pred == expected
+        pred = self.normalizer_es.normalize(test_input, verbose=False)
+        assert pred == expected, f"input: {test_input}"
 
-        if self.normalizer_with_audio:
-            pred_non_deterministic = self.normalizer_with_audio.normalize(
-                test_input, n_tagged=500, punct_post_process=False
+        if self.normalizer_with_audio_es:
+            pred_non_deterministic = self.normalizer_with_audio_es.normalize(
+                test_input, n_tagged=150, punct_post_process=False
             )
-            assert expected in pred_non_deterministic
+            assert expected in pred_non_deterministic, f"input: {test_input}"
```

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_whitelist.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/es/test_word.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/test_ordinal.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,45 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 import pytest
 from nemo_text_processing.inverse_text_normalization.inverse_normalize import InverseNormalizer
 from nemo_text_processing.text_normalization.normalize import Normalizer
 from nemo_text_processing.text_normalization.normalize_with_audio import NormalizerWithAudio
 from parameterized import parameterized
 
 from ..utils import CACHE_DIR, RUN_AUDIO_BASED_TESTS, parse_test_case_file
 
 
-class TestWord:
-    inverse_normalizer_es = InverseNormalizer(lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
+class TestOrdinal:
+    inverse_normalizer = InverseNormalizer(lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
 
-    @parameterized.expand(parse_test_case_file('es/data_inverse_text_normalization/test_cases_word.txt'))
+    @parameterized.expand(parse_test_case_file('es/data_inverse_text_normalization/test_cases_ordinal.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
-    def test_denorm_es(self, test_input, expected):
-        pred = self.inverse_normalizer_es.inverse_normalize(test_input, verbose=False)
+    def test_denorm(self, test_input, expected):
+        pred = self.inverse_normalizer.inverse_normalize(test_input, verbose=False)
         assert pred == expected
 
-    normalizer_es = Normalizer(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
-    normalizer_with_audio_es = (
+    normalizer = Normalizer(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
+    normalizer_with_audio = (
         NormalizerWithAudio(input_case='cased', lang='es', cache_dir=CACHE_DIR, overwrite_cache=False)
         if CACHE_DIR and RUN_AUDIO_BASED_TESTS
         else None
     )
 
-    @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_word.txt'))
+    @parameterized.expand(parse_test_case_file('es/data_text_normalization/test_cases_ordinal.txt'))
     @pytest.mark.run_only_on('CPU')
     @pytest.mark.unit
     def test_norm(self, test_input, expected):
-        pred = self.normalizer_es.normalize(test_input, verbose=False)
-        assert pred == expected, f"input: {test_input}"
+        pred = self.normalizer.normalize(test_input, verbose=False)
+        assert pred in expected
 
-        if self.normalizer_with_audio_es:
-            pred_non_deterministic = self.normalizer_with_audio_es.normalize(
-                test_input, n_tagged=150, punct_post_process=False
+        if self.normalizer_with_audio:
+            pred_non_deterministic = self.normalizer_with_audio.normalize(
+                test_input, n_tagged=500, punct_post_process=False,
             )
-            assert expected in pred_non_deterministic, f"input: {test_input}"
+            assert expected in pred_non_deterministic
```

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_cardinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_decimal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_electronic.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_fraction.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_ordinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_telephone.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_whitelist.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/fr/test_word.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/fr/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_cardinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_decimal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_electronic.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_ordinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_telephone.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_whitelist.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/pt/test_word.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/pt/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/data_text_normalization/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/data_text_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/test_ru_inverse_normalization.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/ru/test_ru_normalization.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/ru/test_ru_normalization.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/es/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_cardinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_decimal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_electronic.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_fraction.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_normalization_with_audio.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_normalization_with_audio.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_ordinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_telephone.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_whitelist.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/sv/test_word.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/sv/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/utils.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,16 +37,28 @@
 def parse_test_case_file(file_name: str):
     """
     Prepares tests pairs for ITN and TN tests
     """
     test_pairs = []
     with open(os.path.dirname(os.path.abspath(__file__)) + os.path.sep + file_name, 'r') as f:
         for line in f:
-            spoken, written = line.split('~')
-            test_pairs.append((spoken, written.strip("\n")))
+            components = line.strip("\n").split("~")
+            spoken = components[0]
+
+            """
+            Some transformations can have multiple correct forms. Instead of
+            asserting against a single expected value, we assert that the
+            output matches any of the correct forms.
+
+                Example:    200 can be "doscientos" or "doscientas" in Spanish
+                Test data:  200~doscientos~doscientas
+                Evaluation: ASSERT "doscientos" in ["doscientos", "doscientas"]
+            """
+            written = components[1] if len(components) == 2 else components[1:]
+            test_pairs.append((spoken, written))
     return test_pairs
 
 
 def get_test_cases_multiple(file_name: str = 'data_text_normalization/en/test_cases_normalize_with_audio.txt'):
     """
     Prepares tests pairs for audio based TN tests
     """
```

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_cardinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_cardinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_decimal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_decimal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_electronic.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_electronic.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_fraction.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_ordinal.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_ordinal.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_telephone.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_telephone.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_time.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_whitelist.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/vi/test_word.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/vi/test_word.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/__init__.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_char.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_char.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_date.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_date.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_fraction.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_fraction.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_math.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_math.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_measure.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_measure.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_money.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_money.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_preprocess.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `nemo_text_processing-0.1.7rc0/tests/nemo_text_processing/zh/test_time.py` & `nemo_text_processing-0.1.8rc0/tests/nemo_text_processing/zh/test_time.py`

 * *Files identical despite different names*

