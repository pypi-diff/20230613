# Comparing `tmp/evals-nightly-1.0.3.dev20230530.tar.gz` & `tmp/evals-nightly-1.0.3.dev20230613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-nightly-1.0.3.dev20230530.tar", last modified: Wed May 31 00:13:44 2023, max compression
+gzip compressed data, was "evals-nightly-1.0.3.dev20230613.tar", last modified: Tue Jun 13 20:51:57 2023, max compression
```

## Comparing `evals-nightly-1.0.3.dev20230530.tar` & `evals-nightly-1.0.3.dev20230613.tar`

### file list

```diff
@@ -1,298 +1,400 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/LICENSE
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5460 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.233058 evals-nightly-1.0.3.dev20230530/evals/
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/api.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/cli/
--rw-r--r--   0 root         (0) root         (0)     5645 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/cli/oaieval.py
--rw-r--r--   0 root         (0) root         (0)     3332 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/cli/oaievalset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/completion_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/cot.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_llm.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_math.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/openai.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/retrieval.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/
--rw-r--r--   0 root         (0) root         (0)     1756 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/fuzzy_match_test.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/includes.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/json_validator.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/match.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/base.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify_utils.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/multiple_choice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/test/
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/test/match.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/translate.py
--rw-r--r--   0 root         (0) root         (0)     6413 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/utils.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/utils_test.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/eval.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/formatting.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/prompt/
--rw-r--r--   0 root         (0) root         (0)     4093 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/prompt/base.py
--rw-r--r--   0 root         (0) root         (0)    18168 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.233058 evals-nightly-1.0.3.dev20230530/evals/registry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/cot.yaml
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/langchain_chains.yaml
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/langchain_llms.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.241059 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/test-modelgraded.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals/registry/evals/
--rw-r--r--   0 root         (0) root         (0)      284 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/2d_movement.yaml
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/aba-mrpc-true-false.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/actors-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/adultery_state_laws.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/afrikaans-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/aime_evaluation.yaml
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/algebra-word-problems.yaml
--rw-r--r--   0 root         (0) root         (0)      451 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ambiguous-sentences.yaml
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/anagrams.yaml
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/arithmetical_puzzles.yaml
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ascii-wordart.yaml
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/atpl_exams.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/balance-chemical-equation.yaml
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/banking77.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/belarusian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/bigrams.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/bitwise.yaml
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/body-movement.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/born-first.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/brazilian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      205 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/building_floorplan.yaml
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/bulgarian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/categorize_with_distractors.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chess-piece-count.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chess.yaml
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chinese_poem.yaml
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chinese_tang_poetries.yaml
--rw-r--r--   0 root         (0) root         (0)      295 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/cissp-study-questions.yaml
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/color_theory_complementary.yaml
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/compare-countries-area.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/complex-replace-characters.yaml
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/connect-4.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/convert-hex-hsl-lightness.yaml
--rw-r--r--   0 root         (0) root         (0)     1719 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/count_intersections_polynomial.yaml
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/count_token_freq_dna.yaml
--rw-r--r--   0 root         (0) root         (0)      387 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/counterfactual-reasoning.yaml
--rw-r--r--   0 root         (0) root         (0)      166 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/countries.yaml
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/crepe.yaml
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/crontab.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/cube-pack.yaml
--rw-r--r--   0 root         (0) root         (0)      179 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/date-booking.yaml
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/date-calculator.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/day-of-week-from-date.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/decrypt-caesar-cipher.yaml
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/detect-hshd.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/determinant.yaml
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/diabetes.yaml
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/diagrammatic_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/dice-rotation-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      199 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/direct-speech-tag.yaml
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/directions.yaml
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/dna-melting-calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/dutch-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/emoji-riddle.yaml
--rw-r--r--   0 root         (0) root         (0)      387 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/emotional-intelligence.yaml
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/escher-sentences.yaml
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/european-date-format-challenge.yaml
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/event-categories.yaml
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/fcc_amateur_extra.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/finance.yaml
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/financial-derivatives.yaml
--rw-r--r--   0 root         (0) root         (0)      181 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/find-letter.yaml
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/find-thirukkural.yaml
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/find_country_from_svg.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/finnish-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/first-letters.yaml
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/food.yaml
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/formal_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      928 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/forth-stack-sim.yaml
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/french-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      361 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/french-part-of-speech.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/gol.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/greek-vocabulary.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/guess-the-singer.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/heart-disease.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hebrew-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hebrew-same-noun-gender.yaml
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hindi_shuddha.yaml
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hindi_upsc.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hindi_words.yaml
--rw-r--r--   0 root         (0) root         (0)      265 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/illinois-law.yaml
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/imperial_date_to_string.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/infiniteloop-match.yaml
--rw-r--r--   0 root         (0) root         (0)     1113 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/integer-sequence-predictions.yaml
--rw-r--r--   0 root         (0) root         (0)      235 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/internal_representations.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/invert_word_wise.yaml
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/invoice_due_date_leap_day_adjustment.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/invoices.yaml
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/irish-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/irony.yaml
--rw-r--r--   0 root         (0) root         (0)      370 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/islands.yaml
--rw-r--r--   0 root         (0) root         (0)      233 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/isosceles-right-triangle.yaml
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/italian-new-words.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/italian-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese-itpassport-exam01.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese-national-medical-exam01.yaml
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_city_name_pronuciation.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_driving_license.yaml
--rw-r--r--   0 root         (0) root         (0)      338 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_number_reading.yaml
--rw-r--r--   0 root         (0) root         (0)      448 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_populer_video_game_title_and_the_publisher.yaml
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/jee-math.yaml
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
--rw-r--r--   0 root         (0) root         (0)      248 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/kanji-idioms.yaml
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/knot-theory.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/korean-consonant-vowel-combination.yaml
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/korean_spelling.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/language.yaml
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/largest_country.yaml
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/last-word-nth.yaml
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/lat_long_identify.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/linear-equations.yaml
--rw-r--r--   0 root         (0) root         (0)      802 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/linear-regression.yaml
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/list_comparison_missing_name.yaml
--rw-r--r--   0 root         (0) root         (0)      456 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logic-liar-paradox.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logic-statements.yaml
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logic.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logical_counting.yaml
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logiqa.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/loss-logic.yaml
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/lunar-calendar.yaml
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mandaliof-table.yaml
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/map-electronic-component-part-to-fact.yaml
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mate-in-one.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/matrix-mult-rows.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/medmcqa.yaml
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mendelian_inheritance.yaml
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/missing-operators.yaml
--rw-r--r--   0 root         (0) root         (0)    14586 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mmlu.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/moral_exceptQA.yaml
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/multi-step-equations.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/multistep-word-problems.yaml
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/music-theory-chord-names.yaml
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/music-theory-chord-notes.yaml
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/music_theory_scale_modes.yaml
--rw-r--r--   0 root         (0) root         (0)     1193 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/naughty_strings.yaml
--rw-r--r--   0 root         (0) root         (0)      361 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/nepali-song-singer.yaml
--rw-r--r--   0 root         (0) root         (0)      340 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/newsology.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/norwegian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/number-pattern.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/number-reading.yaml
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/numbers_game.yaml
--rw-r--r--   0 root         (0) root         (0)      317 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/nutrition.yaml
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ordered-history-events.yaml
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/pararule-plus-multi-step-deductive-reasoning.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/partially_solved_crossword_clues.yaml
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/pattern_identification.yaml
--rw-r--r--   0 root         (0) root         (0)      287 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ph_calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      317 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/physics-interaction.yaml
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/poker_hand_ranks.yaml
--rw-r--r--   0 root         (0) root         (0)      270 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/polish_rhymes_generation.yaml
--rw-r--r--   0 root         (0) root         (0)      277 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/portuguese-sarcasm.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/portuguese-syllable-count.yaml
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/positive-binary-operations.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/probability_questions.yaml
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/python_list_comprehension.yaml
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/qa.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/regex-match.yaml
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/resistor-ohm-calculator.yaml
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/reverse-polish-notation.yaml
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/reverse-string.yaml
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rhetorical-devices.yaml
--rw-r--r--   0 root         (0) root         (0)      255 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rot13.yaml
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rubiks-colors.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rucola.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russe.yaml
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      199 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian-nlp-tasks.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian_medical.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sarcasm.yaml
--rw-r--r--   0 root         (0) root         (0)      338 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/seating_arrangements.yaml
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/security_guide.yaml
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sexagenary-cycle-calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/shape-in-shape.yaml
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/shared-borders.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/simple-knowledge-mongolian.yaml
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/simple-visual-understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sort-numeric.yaml
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/south-african-bands.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/spanish-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/spanish_feminine_noun_masculine_article.yaml
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sql.yaml
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/squares-gpt.yaml
--rw-r--r--   0 root         (0) root         (0)     4472 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/superficial-patterns.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/svg_understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/swap-words.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/swedish-spelling.yaml
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/swedish_sat.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/syntax-check.yaml
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/taxes.yaml
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/tempo_to_measure_count.yaml
--rw-r--r--   0 root         (0) root         (0)     1169 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      400 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-comp-sci.yaml
--rw-r--r--   0 root         (0) root         (0)     1271 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded-generated.yaml
--rw-r--r--   0 root         (0) root         (0)     3040 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test_japanese_units.yaml
--rw-r--r--   0 root         (0) root         (0)      360 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/tetris.yaml
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/three-pt-mapping.yaml
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/time-zone-conversion.yaml
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/track_objects.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/tracking-shuffled-objects.yaml
--rw-r--r--   0 root         (0) root         (0)      174 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ukraine-eit.yaml
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unified-patch.yaml
--rw-r--r--   0 root         (0) root         (0)      307 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unique_combinations.yaml
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unsolvable_questions.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unwanted-rhyming.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/us-tort-law.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/utility_price_parsing.yaml
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/vigenere.yaml
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/vintage_phone_keyboard_decode.yaml
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/which-is-heavier.yaml
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/wkt_understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/word_vector_over_reliance.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      492 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/best.yaml
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 root         (0) root         (0)     1157 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 root         (0) root         (0)     2564 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 root         (0) root         (0)      887 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/regression-equation.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/rhyming.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/security.yaml
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/sql.yaml
--rw-r--r--   0 root         (0) root         (0)     9547 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals/utils/
--rw-r--r--   0 root         (0) root         (0)     2136 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/utils/api_utils.py
--rw-r--r--   0 root         (0) root         (0)      713 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/utils/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11480 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5697 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/api.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/cli/
+-rw-r--r--   0 root         (0) root         (0)     6454 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/cli/oaieval.py
+-rw-r--r--   0 root         (0) root         (0)     3863 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/cli/oaievalset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/cot.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/openai.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/fuzzy_match_test.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/includes.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/includes_test.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/json_validator.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/json_validator_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/match.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/match_test.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/lambada.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/multiple_choice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/test/
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/test/match.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/translate.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/utils.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/eval.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/formatting.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/prompt/
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/prompt/base.py
+-rw-r--r--   0 root         (0) root         (0)    18168 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.049988 evals-nightly-1.0.3.dev20230613/evals/registry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.057988 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.057988 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/logiqa-logical-reasoning-plus.yaml
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/pointer-value-retrieval.yaml
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/raven-matrices.yaml
+-rw-r--r--   0 root         (0) root         (0)      560 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/test-modelgraded.yaml
+-rw-r--r--   0 root         (0) root         (0)      613 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/ukraine-gec.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.093990 evals-nightly-1.0.3.dev20230613/evals/registry/evals/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/2d_movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/3d_globe_movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/abstract-causal-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/adultery_state_laws.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/afrikaans-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/aime_evaluation.yaml
+-rw-r--r--   0 root         (0) root         (0)      457 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/algebra-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      418 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/allergen-information.yaml
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/alternate-numeral-systems.yaml
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ambiguous-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      229 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/arc.yaml
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/arithmetical_puzzles.yaml
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ascii-wordart.yaml
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/asl-classifiers.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/atpl_exams.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/banking77.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/beam-analysis.yaml
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-grammar.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-proverbs.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-russian-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-syllable-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-synonyms.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/bitwise.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/body-movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/brazilian_laws.yaml
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/building_floorplan.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/canto_wu_pronunciation.yaml
+-rw-r--r--   0 root         (0) root         (0)      355 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/canto_wu_pronunciation_fewshot.yaml
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cardinal-directions.yaml
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/categorize_with_distractors.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chess.yaml
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_homonym.yaml
+-rw-r--r--   0 root         (0) root         (0)      178 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_poem.yaml
+-rw-r--r--   0 root         (0) root         (0)      190 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_song_ci.yaml
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_tang_poetries.yaml
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_zodiac.yaml
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cissp-study-questions.yaml
+-rw-r--r--   0 root         (0) root         (0)      372 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/code_combination.yaml
+-rw-r--r--   0 root         (0) root         (0)      343 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/color_theory_complementary.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/compare-countries-area.yaml
+-rw-r--r--   0 root         (0) root         (0)      223 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/complex-analogies-en-ru.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/comprehensive-graph-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/context-free-grammar.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/count_intersections_polynomial.yaml
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/count_token_freq_dna.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/counterfactual-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/countries.yaml
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cricket_situations.yaml
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/crontab.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cybersecurity-filepaths.yaml
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/date-booking.yaml
+-rw-r--r--   0 root         (0) root         (0)      192 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/date-calculator.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/day-of-week-from-date.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/detect-hshd.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/diabetes.yaml
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/dice-rotation-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/direct-speech-tag.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/directions.yaml
+-rw-r--r--   0 root         (0) root         (0)      316 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/dna-melting-calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/dutch-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/emoji-riddle.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/escher-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/euler_problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/european-date-format-challenge.yaml
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/event-categories.yaml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/fcc_amateur_extra.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/finance.yaml
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/financial-derivatives.yaml
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/find-letter.yaml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/find-thirukkural.yaml
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/find_country_from_svg.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/finnish-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/food.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/formal-grammar-to-regex.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      928 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/french-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/french-part-of-speech.yaml
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/game-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/geometry_puzzle.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/german-part-of-speech.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/gol.yaml
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/gpt-protocol-buffers.yaml
+-rw-r--r--   0 root         (0) root         (0)      404 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/greek-nt-manuscripts.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/greek-vocabulary.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/guess-the-singer.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hebrew-bible.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hebrew-same-noun-gender.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hindi_shuddha.yaml
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hindi_upsc.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hindi_words.yaml
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/historical-kana-orthography-reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      313 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/human-safety.yaml
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/iambic-pentameter.yaml
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/indonesian_numbers.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/integer-sequence-predictions.yaml
+-rw-r--r--   0 root         (0) root         (0)      235 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/internal_representations.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/invert_word_wise.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/invoice_due_date_leap_day_adjustment.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/invoices.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/irish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/irony.yaml
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/islands.yaml
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/isosceles-right-triangle.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/italian-new-words.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/italian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese-itpassport-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese-national-medical-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese-national-medical-exam02.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_city_name_pronuciation.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_driving_license.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_number_reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_populer_video_game_title_and_the_publisher.yaml
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/jee-math.yaml
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/json_patch_object.yaml
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/kanji-idioms.yaml
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/knot-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean-consonant-vowel-combination.yaml
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean-phonetics.yaml
+-rw-r--r--   0 root         (0) root         (0)      293 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean_dialects.yaml
+-rw-r--r--   0 root         (0) root         (0)      191 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean_spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean_yaminjeongeum.yaml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/language.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/largest_country.yaml
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/linear-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/linear-regression.yaml
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/list_comparison_missing_name.yaml
+-rw-r--r--   0 root         (0) root         (0)      814 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-grid-eval.yaml
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-liar-paradox.yaml
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-riddles.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic_and_probability.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logical_counting.yaml
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logiqa-logical-reasoning-plus.yaml
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/loss-logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/lunar-calendar.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mandaliof-table.yaml
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mapping_to_matricies.yaml
+-rw-r--r--   0 root         (0) root         (0)      243 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mate-in-one.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/matrix-mult-rows.yaml
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/medication_dose.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/medmcqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 root         (0) root         (0)      337 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/missing-operators.yaml
+-rw-r--r--   0 root         (0) root         (0)    14586 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mmlu.yaml
+-rw-r--r--   0 root         (0) root         (0)      313 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/monthly_metric_comparison.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/multi-step-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/multistep-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music-theory-chord-names.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music-theory-chord-notes.yaml
+-rw-r--r--   0 root         (0) root         (0)      874 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music_theory_scale_modes.yaml
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/nepali-song-singer.yaml
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/newsology.yaml
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/next-val-series.yaml
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/nfl-point-combinations.yaml
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/non-compound-names.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/norwegian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/numbers_game.yaml
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/numeral-type-comparisons.yaml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/nutrition.yaml
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ordered-history-events.yaml
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/override-system-instruction.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pantone_to_hex.yaml
+-rw-r--r--   0 root         (0) root         (0)      502 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/parable-to-moral-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pararule-plus-multi-step-deductive-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/passing-balls.yaml
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 root         (0) root         (0)      287 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ph_calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      429 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/phonetics-identify-words-needing-missing-gpcs.yaml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/physics-interaction.yaml
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pointer-value-retrieval.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/points-on-line.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/poker_analysis.yaml
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/polish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/polish-syllable-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/polish_rhymes_generation.yaml
+-rw-r--r--   0 root         (0) root         (0)      579 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/population_span_extraction.yaml
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/portuguese-sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/portuguese-syllable-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/positive-binary-operations.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/probability_questions.yaml
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/product-matching.yaml
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/prompt-injection.yaml
+-rw-r--r--   0 root         (0) root         (0)      235 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pure_korean.yaml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/python_list_comprehension.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/qa.yaml
+-rw-r--r--   0 root         (0) root         (0)      219 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/quartz.yaml
+-rw-r--r--   0 root         (0) root         (0)      380 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rare-and-loanwords-dutch-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)    14285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/raven-matrices.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rectangles.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/resistor-ohm-calculator.yaml
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/resource_id_extraction.yaml
+-rw-r--r--   0 root         (0) root         (0)      321 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/reverse-polish-notation.yaml
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/reverse-sort-words-eng.yaml
+-rw-r--r--   0 root         (0) root         (0)      378 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rhetorical-devices.yaml
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rock-climbing.yaml
+-rw-r--r--   0 root         (0) root         (0)      255 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 root         (0) root         (0)      468 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ru_rhymes.yaml
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rubiks-colors.yaml
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russe.yaml
+-rw-r--r--   0 root         (0) root         (0)      298 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-english-homonym-context-resolution.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-verse.yaml
+-rw-r--r--   0 root         (0) root         (0)      190 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian_medical.yaml
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian_sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/seating_arrangements.yaml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/security_guide.yaml
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sexagenary-cycle-calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/shape-in-shape.yaml
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/shared-borders.yaml
+-rw-r--r--   0 root         (0) root         (0)      328 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/shopping_discount_comparison.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple-knowledge-mongolian.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple-visual-understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple_math.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple_physics_engine.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sindarin-fluency.yaml
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/soc_codes.yaml
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/solve-for-variable.yaml
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sort-numeric.yaml
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/south-african-bands.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/spanish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/spanish_feminine_noun_masculine_article.yaml
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/split_chinese_characters.yaml
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/squares-gpt.yaml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/stats-tests.yaml
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/superficial-patterns.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/svg_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/swap-words.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/swedish_sat.yaml
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/syllables_long_words.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/syntax-check.yaml
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/tempo_to_measure_count.yaml
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test_japanese_radical.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test_japanese_units.yaml
+-rw-r--r--   0 root         (0) root         (0)      360 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/tetris.yaml
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/three-pt-mapping.yaml
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/time-zone-conversion.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/track_objects.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/tracking-shuffled-objects.yaml
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/turkish_characters.yaml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 root         (0) root         (0)     6692 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ukraine-gec.yaml
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ukraine_electronic_petitions.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unified-patch.yaml
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unique_combinations.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unsolvable_questions.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unwanted-rhyming.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/utility_price_parsing.yaml
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/vigenere.yaml
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/vintage_phone_keyboard_decode.yaml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/which-is-heavier.yaml
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/wkt_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/word_vector_over_reliance.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.093990 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/iambic_pentameter.yaml
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/regression-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/rhyming.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)    10309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.093990 evals-nightly-1.0.3.dev20230613/evals/utils/
+-rw-r--r--   0 root         (0) root         (0)     2136 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/api_utils.py
+-rw-r--r--   0 root         (0) root         (0)      713 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16118 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      765 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/setup.cfg
```

### Comparing `evals-nightly-1.0.3.dev20230530/LICENSE` & `evals-nightly-1.0.3.dev20230613/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/README.md` & `evals-nightly-1.0.3.dev20230613/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,20 +34,23 @@
 
 To run evals, you will need to set up and specify your OpenAI API key. You can generate one at <https://platform.openai.com/account/api-keys>. After you obtain an API key, specify it using the `OPENAI_API_KEY` environment variable. **Please be aware of the [costs](https://openai.com/pricing) associated with using the API when running evals.**
 
 **Minimum Required Version: Python 3.9**
 
 ### Downloading evals
 
-Our Evals registry is stored using [Git-LFS](https://git-lfs.com/). Once you have downloaded and installed LFS, you can fetch the evals with:
+Our Evals registry is stored using [Git-LFS](https://git-lfs.com/). Once you have downloaded and installed LFS, you can fetch the evals (from within your local copy of the evals repo) with:
 ```sh
+cd evals
 git lfs fetch --all
 git lfs pull
 ```
 
+This will populate all the pointer files under `evals/registry/data`.
+
 You may just want to fetch data for a select eval. You can achieve this via:
 ```sh
 git lfs fetch --include=evals/registry/data/${your eval}
 git lfs pull
 ```
 
 ### Making evals
@@ -56,14 +59,20 @@
 
 ```sh
 pip install -e .
 ```
 
 Using `-e`, changes you make to your eval will be reflected immediately without having to reinstall.
 
+Optionally, you can install the formatters for pre-committing with:
+
+```sh
+pip install -e .[formatters]
+```
+
 ### Running evals
 
 If you don't want to contribute new evals, but simply want to run them locally, you can install the evals package via pip:
 
 ```sh
 pip install evals
 ```
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/api.py` & `evals-nightly-1.0.3.dev20230613/evals/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         prompt: Union[str, OpenAICreateChatPrompt],
         **kwargs,
     ) -> CompletionResult:
         """
         ARGS
         ====
         `prompt`: Either a `Prompt` object or a raw prompt that will get wrapped in
-            the approriate `Prompt` class.
+            the appropriate `Prompt` class.
         `kwargs`: Other arguments passed to the API.
 
         RETURNS
         =======
         The result of the API call.
         The prompt that was fed into the API call as a str.
         """
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/base.py` & `evals-nightly-1.0.3.dev20230613/evals/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/cli/oaieval.py` & `evals-nightly-1.0.3.dev20230613/evals/cli/oaieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 This file defines the `oaieval` CLI for running evals.
 """
 import argparse
 import logging
 import shlex
 import sys
-from typing import Any, Mapping, Optional
+from typing import Any, Mapping, Optional, Union, cast
 
 import openai
 
 import evals
 import evals.api
 import evals.base
 import evals.record
+from evals.eval import Eval
 from evals.registry import Registry
 
 logger = logging.getLogger(__name__)
 
 
-def _purple(str):
+def _purple(str: str) -> str:
     return f"\033[1;35m{str}\033[0m"
 
 
 def get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="Run evals through the API")
     parser.add_argument(
         "completion_fn",
@@ -37,24 +38,46 @@
     parser.add_argument("--seed", type=int, default=20220722)
     parser.add_argument("--user", type=str, default="")
     parser.add_argument("--record_path", type=str, default=None)
     parser.add_argument(
         "--log_to_file", type=str, default=None, help="Log to a file instead of stdout"
     )
     parser.add_argument(
-        "--registry_path", type=str, default=None, action="append", help="Path to the registry"
+        "--registry_path",
+        type=str,
+        default=None,
+        action="append",
+        help="Path to the registry",
     )
     parser.add_argument("--debug", action=argparse.BooleanOptionalAction, default=False)
     parser.add_argument("--local-run", action=argparse.BooleanOptionalAction, default=True)
     parser.add_argument("--dry-run", action=argparse.BooleanOptionalAction, default=False)
     parser.add_argument("--dry-run-logging", action=argparse.BooleanOptionalAction, default=True)
     return parser
 
 
-def run(args, registry: Optional[Registry] = None):
+class OaiEvalArguments(argparse.Namespace):
+    completion_fn: str
+    eval: str
+    extra_eval_params: str
+    max_samples: Optional[int]
+    cache: bool
+    visible: Optional[bool]
+    seed: int
+    user: str
+    record_path: Optional[str]
+    log_to_file: Optional[str]
+    registry_path: Optional[str]
+    debug: bool
+    local_run: bool
+    dry_run: bool
+    dry_run_logging: bool
+
+
+def run(args: OaiEvalArguments, registry: Optional[Registry] = None) -> str:
     if args.debug:
         logging.getLogger().setLevel(logging.DEBUG)
 
     visible = args.visible if args.visible is not None else (args.max_samples is None)
 
     if args.max_samples is not None:
         evals.eval.set_max_samples(args.max_samples)
@@ -79,46 +102,53 @@
         "command": " ".join(map(shlex.quote, sys.argv)),
         "initial_settings": {
             "visible": visible,
         },
     }
 
     eval_name = eval_spec.key
+    if eval_name is None:
+        raise Exception("you must provide a eval name")
+
     run_spec = evals.base.RunSpec(
         completion_fns=completion_fns,
         eval_name=eval_name,
         base_eval=eval_name.split(".")[0],
         split=eval_name.split(".")[1],
         run_config=run_config,
         created_by=args.user,
     )
     if args.record_path is None:
         record_path = f"/tmp/evallogs/{run_spec.run_id}_{args.completion_fn}_{args.eval}.jsonl"
     else:
         record_path = args.record_path
+
+    recorder: evals.record.RecorderBase
     if args.dry_run:
         recorder = evals.record.DummyRecorder(run_spec=run_spec, log=args.dry_run_logging)
     elif args.local_run:
         recorder = evals.record.LocalRecorder(record_path, run_spec=run_spec)
     else:
         recorder = evals.record.Recorder(record_path, run_spec=run_spec)
 
-    api_extra_options = {}
+    api_extra_options: dict[str, Any] = {}
     if not args.cache:
         api_extra_options["cache_level"] = 0
 
     run_url = f"{run_spec.run_id}"
     logger.info(_purple(f"Run started: {run_url}"))
 
-    def parse_extra_eval_params(param_str: Optional[str]) -> Mapping[str, Any]:
+    def parse_extra_eval_params(
+        param_str: Optional[str],
+    ) -> Mapping[str, Union[str, int, float]]:
         """Parse a string of the form "key1=value1,key2=value2" into a dict."""
         if not param_str:
             return {}
 
-        def to_number(x):
+        def to_number(x: str) -> Union[int, float, str]:
             try:
                 return int(x)
             except:
                 pass
             try:
                 return float(x)
             except:
@@ -127,15 +157,15 @@
 
         str_dict = dict(kv.split("=") for kv in param_str.split(","))
         return {k: to_number(v) for k, v in str_dict.items()}
 
     extra_eval_params = parse_extra_eval_params(args.extra_eval_params)
 
     eval_class = registry.get_class(eval_spec)
-    eval = eval_class(
+    eval: Eval = eval_class(
         completion_fns=completion_fn_instances,
         seed=args.seed,
         name=eval_name,
         registry=registry,
         **extra_eval_params,
     )
     result = eval.run(recorder)
@@ -146,23 +176,25 @@
 
     logger.info("Final report:")
     for key, value in result.items():
         logger.info(f"{key}: {value}")
     return run_spec.run_id
 
 
-def main():
+def main() -> None:
     parser = get_parser()
-    args = parser.parse_args(sys.argv[1:])
+    args = cast(OaiEvalArguments, parser.parse_args(sys.argv[1:]))
     logging.basicConfig(
         format="[%(asctime)s] [%(filename)s:%(lineno)d] %(message)s",
         level=logging.INFO,
         filename=args.log_to_file if args.log_to_file else None,
     )
     logging.getLogger("openai").setLevel(logging.WARN)
-    if hasattr(openai.error, "set_display_cause"):
-        openai.error.set_display_cause()
+
+    # TODO)) why do we need this?
+    if hasattr(openai.error, "set_display_cause"):  # type: ignore
+        openai.error.set_display_cause()  # type: ignore
     run(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/cli/oaievalset.py` & `evals-nightly-1.0.3.dev20230613/evals/cli/oaievalset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 This file defines the `oaievalset` CLI for running eval sets.
 """
 import argparse
 import json
+import logging
 import subprocess
 from pathlib import Path
-from typing import Optional
+from typing import Optional, cast
 
 from evals.registry import Registry
 
 Task = list[str]
+logger = logging.getLogger(__name__)
 
 
 class Progress:
     def __init__(self, file: str) -> None:
         self.file = Path(file)
         self.completed: list[Task] = []
 
@@ -57,25 +59,42 @@
         action=argparse.BooleanOptionalAction,
         default=True,
         help="Exit if any oaieval command fails.",
     )
     return parser
 
 
+class OaiEvalSetArguments(argparse.Namespace):
+    model: str
+    eval_set: str
+    resume: bool
+    exit_on_error: bool
+
+
 def run(
-    args, unknown_args, registry: Optional[Registry] = None, run_command: str = "oaieval"
+    args: OaiEvalSetArguments,
+    unknown_args: list[str],
+    registry: Optional[Registry] = None,
+    run_command: str = "oaieval",
 ) -> None:
     registry = registry or Registry()
     commands: list[Task] = []
-    eval_set = registry.get_eval_set(args.eval_set)
-    for eval in registry.get_evals(eval_set.evals):
-        command = [run_command, args.model, eval.key] + unknown_args
-        if command in commands:
-            continue
-        commands.append(command)
+    eval_set = registry.get_eval_set(args.eval_set) if args.eval_set else None
+    if eval_set:
+        for index, eval in enumerate(registry.get_evals(eval_set.evals)):
+            if not eval or not eval.key:
+                logger.debug("The eval #%d in eval_set is not valid", index)
+
+            command = [run_command, args.model, eval.key] + unknown_args
+            if command in commands:
+                continue
+            commands.append(command)
+    else:
+        logger.warning("No eval set found for %s", args.eval_set)
+
     num_evals = len(commands)
 
     progress = Progress(f"/tmp/oaievalset/{args.model}.{args.eval_set}.progress.txt")
     if args.resume and progress.load():
         print(f"Loaded progress from {progress.file}")
         print(f"{len(progress.completed)}/{len(commands)} evals already completed:")
         for item in progress.completed:
@@ -96,12 +115,12 @@
 
     print(highlight("All done!"))
 
 
 def main() -> None:
     parser = get_parser()
     args, unknown_args = parser.parse_known_args()
-    run(args, unknown_args)
+    run(cast(OaiEvalSetArguments, args), unknown_args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/completion_fns/cot.py` & `evals-nightly-1.0.3.dev20230613/evals/completion_fns/cot.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_llm.py` & `evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_math.py` & `evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_math.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/completion_fns/openai.py` & `evals-nightly-1.0.3.dev20230613/evals/completion_fns/openai.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/completion_fns/retrieval.py` & `evals-nightly-1.0.3.dev20230613/evals/completion_fns/retrieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/data.py` & `evals-nightly-1.0.3.dev20230613/evals/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,18 +67,28 @@
                 )
             else:
                 return open_fn(filename, mode=mode)
     except Exception as e:
         raise RuntimeError(f"Failed to open: {filename}") from e
 
 
+def _decode_json(line, path, line_number):
+    try:
+        return json.loads(line)
+    except json.JSONDecodeError as e:
+        custom_error_message = f"Error parsing JSON on line {line_number}: {e.msg} at {path}:{line_number}:{e.colno}"
+        logger.error(custom_error_message)
+        raise ValueError(custom_error_message) from None
+
 def _get_jsonl_file(path):
     logger.info(f"Fetching {path}")
+    data = []
     with open_by_file_pattern(path, mode="r") as f:
-        return list(map(json.loads, f.readlines()))
+        return [_decode_json(line, path, i + 1) for i, line in enumerate(f)]
+
 
 
 def _get_json_file(path):
     logger.info(f"Fetching {path}")
     with open_by_file_pattern(path, mode="r") as f:
         return json.loads(f.read())
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/fuzzy_match.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/fuzzy_match.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,32 +8,37 @@
 
 class FuzzyMatch(evals.Eval):
     def __init__(
         self,
         completion_fns: list[CompletionFn],
         samples_jsonl: str,
         *args,
-        max_tokens: int = 500,
+        max_tokens: int = 100,
         **kwargs,
     ):
         super().__init__(completion_fns, *args, **kwargs)
         assert len(completion_fns) == 1, "FuzzyMatch only supports one completion fn"
         self.max_tokens = max_tokens
         self.samples_jsonl = samples_jsonl
 
     def eval_sample(self, test_sample, rng):
         del rng
+
+        assert isinstance(test_sample, dict), "sample must be a dict"
+        assert "input" in test_sample, "sample must have an 'input' key"
+        assert "ideal" in test_sample, "sample must have an 'ideal' key"
+
         prompt, correct_answers = test_sample["input"], test_sample["ideal"]
         if not isinstance(correct_answers, list):
             correct_answers = [correct_answers]
 
         result = self.completion_fn(
             prompt=prompt,
             temperature=0.0,  # Q: why are these hardcoded?
-            max_tokens=100,
+            max_tokens=self.max_tokens,
         )
         sampled = result.get_completions()[0]
 
         matches = [utils.fuzzy_match(sampled, correct_answer) for correct_answer in correct_answers]
 
         evals.record.record_match(
             True in matches,
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/includes.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/includes.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     ):
         super().__init__(completion_fns, *args, **kwargs)
         assert len(completion_fns) == 1, "Includes only supports one completion fn"
         self.samples_jsonl = samples_jsonl
         self.ignore_case = ignore_case
 
     def eval_sample(self, sample: Any, *_):
+        assert isinstance(sample, dict), "sample must be a dict"
+        assert "input" in sample, "sample must have an 'input' key"
+        assert "ideal" in sample, "sample must have an 'ideal' key"
+
         prompt = sample["input"]
         result = self.completion_fn(
             prompt=prompt,
         )
         sampled = result.get_completions()[0]
 
         ideal = sample["ideal"]
@@ -32,24 +36,22 @@
             ideal = [ideal]
 
         assert isinstance(ideal, list) and all(
             isinstance(i, str) for i in ideal
         ), "ideal must be a list of strings"
 
         includes_answer = any(
-            [
-                utils.get_answer(sampled, ref, self.ignore_case) is not None
-                for ref in ideal
-            ]
+            [utils.get_answer(sampled, ref, self.ignore_case) is not None for ref in ideal]
         )
         evals.record.record_match(
             includes_answer, expected=sample["ideal"], picked=sampled, sampled=sampled
         )
         return includes_answer
 
     def run(self, recorder):
         samples = self.get_samples()
         self.eval_all_samples(recorder, samples)
         events = recorder.get_events("match")
         return {
             "accuracy": evals.metrics.get_accuracy(events),
+            "boostrap_std": evals.metrics.get_bootstrap_accuracy_std(events),
         }
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/json_validator.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/json_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,26 @@
         **kwargs,
     ):
         super().__init__(completion_fns, *args, **kwargs)
         assert len(completion_fns) == 1, "JsonValidator only supports one completion fn"
         self.samples_jsonl = samples_jsonl
 
     def eval_sample(self, sample: Any, *_):
+        assert isinstance(sample, dict), "sample must be a dict"
+        assert "input" in sample, "sample must have an 'input' key"
+
         prompt = sample["input"]
         result = self.completion_fn(
             prompt=prompt,
             temperature=0.0,
         )
         sampled = result.get_completions()[0]
         return evals.record.record_match(is_valid_json(sampled), expected=None, picked=sampled)
 
     def run(self, recorder):
         samples = self.get_samples()
         self.eval_all_samples(recorder, samples)
         events = recorder.get_events("match")
         return {
             "accuracy": evals.metrics.get_accuracy(events),
+            "boostrap_std": evals.metrics.get_bootstrap_accuracy_std(events),
         }
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/match.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/match.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,21 @@
         self.num_few_shot = num_few_shot
         if self.num_few_shot > 0:
             assert few_shot_jsonl is not None, "few shot requires few shot sample dataset"
             self.few_shot_jsonl = few_shot_jsonl
             self.few_shot = evals.get_jsonl(self.few_shot_jsonl)
 
     def eval_sample(self, sample: Any, *_):
+        assert isinstance(sample, dict), "sample must be a dict"
+        assert "input" in sample, "sample must have an 'input' key"
+        assert "ideal" in sample, "sample must have an 'ideal' key"
+        assert isinstance(sample["ideal"], str) or isinstance(
+            sample["ideal"], list
+        ), "sample['ideal'] must be a string or list of strings"
+
         prompt = sample["input"]
         if self.num_few_shot > 0:
             assert is_chat_prompt(sample["input"]), "few shot requires chat prompt"
             prompt = sample["input"][:-1]
             for s in self.few_shot[: self.num_few_shot]:
                 prompt += s["sample"]
             prompt += sample["input"][-1:]
@@ -50,8 +57,9 @@
 
     def run(self, recorder):
         samples = self.get_samples()
         self.eval_all_samples(recorder, samples)
         events = recorder.get_events("match")
         return {
             "accuracy": evals.metrics.get_accuracy(events),
+            "boostrap_std": evals.metrics.get_bootstrap_accuracy_std(events),
         }
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/base.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify_utils.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/multiple_choice.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/test/match.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/test/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/translate.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/translate.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/utils.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/elsuite/utils_test.py` & `evals-nightly-1.0.3.dev20230613/evals/elsuite/utils_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/eval.py` & `evals-nightly-1.0.3.dev20230613/evals/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
         self.completion_fns = completion_fns
         self.seed = seed
         self.name = name
         self.registry = registry or Registry()
         self.samples_jsonl = samples_jsonl
 
+    @abc.abstractmethod
     def eval_sample(self, sample: Any, rng: random.Random):
         raise NotImplementedError()
 
     @property
     def completion_fn(self) -> CompletionFn:
         """Helper for more ergonomic access to a single CompletionFn."""
         return self.completion_fns[0]
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/formatting.py` & `evals-nightly-1.0.3.dev20230613/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/metrics.py` & `evals-nightly-1.0.3.dev20230613/evals/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,71 +6,66 @@
 
 import numpy as np
 
 from evals.record import Event
 
 
 def get_accuracy(events: Sequence[Event]) -> float:
-    num_correct = 0
-    num_total = 0
-    for event in events:
-        num_total += 1
-        num_correct += int(event.data["correct"])
+    num_correct = sum(int(event.data["correct"]) for event in events)
+    num_total = len(events)
     if num_total == 0:
         return float("nan")
     else:
         return num_correct / num_total
 
 
-def get_bootstrap_accuracy_std(events: Sequence[Event], num_samples: int = 1000):
+def get_bootstrap_accuracy_std(events: Sequence[Event], num_samples: int = 1000) -> float:
     vals = [m.data["correct"] for m in events]
-    return np.std([np.mean(random.sample(vals, len(vals) // 2)) for _ in range(1000)])
+    return np.std([np.mean(random.sample(vals, len(vals) // 2)) for _ in range(num_samples)])
 
 
 def get_confusion_matrix(
-    matches: Sequence[Event], class_labels: Optional[Set] = None
+        matches: Sequence[Event], class_labels: Optional[Set] = None
 ) -> np.ndarray:
-    labels = set()
-    for match in matches:
-        labels.add(match.data["expected"])
+    labels = {match.data["expected"] for match in matches}
     if class_labels is None:
         labels = {label: i for i, label in enumerate(sorted(labels))}
     else:
         assert labels.issubset(class_labels)
         labels = {label: i for i, label in enumerate(class_labels)}
     result = np.zeros((len(labels), len(labels) + 1), dtype=int)
     for match in matches:
         i = labels[match.data["expected"]]
         j = labels.get(match.data["picked"], len(labels))
         result[i, j] += 1
     return result
 
 
-def compute_matthew_corr(confusion_matrix):
+def compute_matthew_corr(confusion_matrix: np.ndarray) -> float:
     assert confusion_matrix.shape == (2, 3), f"Got shape: {confusion_matrix.shape}"
     r = confusion_matrix[:, :2]
     r[:, 0] += confusion_matrix[:, 2]
     return (r[1, 1] * r[0, 0] - r[1, 0] * r[0, 1]) / np.sqrt(
         r[1, :].sum() * r[0, :].sum() * r[:, 0].sum() * r[:, 1].sum()
     )
 
 
-def compute_precision(confusion_matrix, idx=0):
+def compute_precision(confusion_matrix: np.ndarray, idx: int = 0) -> float:
     return confusion_matrix[idx, idx] / confusion_matrix[:, idx].sum()
 
 
-def compute_recall(confusion_matrix, idx=0):
+def compute_recall(confusion_matrix: np.ndarray, idx: int = 0) -> float:
     return confusion_matrix[idx, idx] / confusion_matrix[idx, :].sum()
 
 
-def compute_f_score(confusion_matrix, idx=0, beta=1.0):
+def compute_f_score(confusion_matrix: np.ndarray, idx: int = 0, beta: float = 1.0) -> float:
     precision = compute_precision(confusion_matrix, idx=idx)
     recall = compute_recall(confusion_matrix, idx=idx)
     return (1 + beta**2) * (precision * recall) / (beta**2 * precision + recall)
 
 
-def compute_averaged_f_score(confusion_matrix, beta=1.0, average="macro"):
+def compute_averaged_f_score(confusion_matrix: np.ndarray, beta: float = 1.0, average: str = "macro") -> float:
     assert average in ["macro"]
     f_scores = []
     for i in range(confusion_matrix.shape[0]):
         f_scores.append(compute_f_score(confusion_matrix, idx=i, beta=beta))
     return np.array(f_scores).mean()
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/prompt/base.py` & `evals-nightly-1.0.3.dev20230613/evals/prompt/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/record.py` & `evals-nightly-1.0.3.dev20230613/evals/record.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/langchain_llms.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/langchain_llms.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/stock-options.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/categorize_with_distractors.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/categorize_with_distractors.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/coqa-ex.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/coqa-ex.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/forth-stack-sim.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/forth-stack-sim.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/integer-sequence-predictions.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/integer-sequence-predictions.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/knot-theory.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/knot-theory.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/linear-regression.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/linear-regression.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/lunar-calendar.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/lunar-calendar.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/manga-translation.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/manga-translation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/mmlu.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/mmlu.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/naughty_strings.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/naughty_strings.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/sql.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/stock-options.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-basic.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-basic.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/closedqa.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/closedqa.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/fact.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/fact.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/humor.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/humor.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/regression-equation.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/regression-equation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/sql.yaml` & `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/registry.py` & `evals-nightly-1.0.3.dev20230613/evals/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import difflib
 import functools
 import logging
 import os
 import re
 from functools import cached_property
 from pathlib import Path
-from typing import Any, Iterator, Optional, Sequence, Type, Union
+from typing import Any, Iterator, Optional, Sequence, Type, TypeVar, Union
 
 import openai
 import yaml
 
 from evals import OpenAIChatCompletionFn, OpenAICompletionFn
 from evals.api import CompletionFn, DummyCompletionFn
 from evals.base import BaseEvalSpec, CompletionFnSpec, EvalSetSpec, EvalSpec
@@ -69,24 +69,34 @@
     "gpt-4",
     "gpt-4-0314",
     "gpt-4-32k",
     "gpt-4-32k-0314",
 }
 
 
+T = TypeVar("T")
+RawRegistry = dict[str, Any]
+
+
 class Registry:
     def __init__(self, registry_paths: Sequence[Union[str, Path]] = DEFAULT_PATHS):
         self._registry_paths = [Path(p) if isinstance(p, str) else p for p in registry_paths]
 
-    def add_registry_paths(self, paths: list[Union[str, Path]]):
+    def add_registry_paths(self, paths: list[Union[str, Path]]) -> None:
         self._registry_paths.extend([Path(p) if isinstance(p, str) else p for p in paths])
 
     @cached_property
-    def api_model_ids(self):
-        return [m["id"] for m in openai.Model.list()["data"]]
+    def api_model_ids(self) -> list[str]:
+        try:
+            return [m["id"] for m in openai.Model.list()["data"]]
+        except openai.error.OpenAIError as err:
+            # Errors can happen when running eval with completion function that uses custom
+            # API endpoints and authentication mechanisms.
+            logger.warning(f"Could not fetch API model IDs from OpenAI API: {err}")
+            return []
 
     def make_completion_fn(self, name: str) -> CompletionFn:
         """
         Create a CompletionFn. The name can be one of the following formats:
         1. openai-model-id (e.g. "gpt-3.5-turbo")
         2. completion-fn-id (from the registry)
         """
@@ -109,28 +119,30 @@
             spec.args = {}
 
         spec.args["registry"] = self
         instance = make_object(spec.cls)(**spec.args or {})
         assert isinstance(instance, CompletionFn), f"{name} must be a CompletionFn"
         return instance
 
-    def get_class(self, spec: dict) -> Any:
+    def get_class(self, spec: EvalSpec) -> Any:
         return make_object(spec.cls, **(spec.args if spec.args else {}))
 
-    def _dereference(self, name: str, d: dict, object: str, type: Type, **kwargs: dict) -> dict:
+    def _dereference(
+        self, name: str, d: RawRegistry, object: str, type: Type[T], **kwargs: dict
+    ) -> Optional[T]:
         if not name in d:
             logger.warning(
                 (
                     f"{object} '{name}' not found. "
                     f"Closest matches: {difflib.get_close_matches(name, d.keys(), n=5)}"
                 )
             )
             return None
 
-        def get_alias():
+        def get_alias() -> Optional[str]:
             if isinstance(d[name], str):
                 return d[name]
             if isinstance(d[name], dict) and "id" in d[name]:
                 return d[name]["id"]
             return None
 
         logger.debug(f"Looking for {name}")
@@ -147,72 +159,72 @@
             spec.update(kwargs)
 
         try:
             return type(**spec)
         except TypeError as e:
             raise TypeError(f"Error while processing {object} '{name}': {e}")
 
-    def get_modelgraded_spec(self, name: str, **kwargs: dict) -> dict[str, Any]:
+    def get_modelgraded_spec(self, name: str, **kwargs: dict) -> Optional[ModelGradedSpec]:
         assert name in self._modelgraded_specs, (
             f"Modelgraded spec {name} not found. "
             f"Closest matches: {difflib.get_close_matches(name, self._modelgraded_specs.keys(), n=5)}"
         )
         return self._dereference(
             name, self._modelgraded_specs, "modelgraded spec", ModelGradedSpec, **kwargs
         )
 
-    def get_completion_fn(self, name: str) -> CompletionFnSpec:
+    def get_completion_fn(self, name: str) -> Optional[CompletionFnSpec]:
         return self._dereference(name, self._completion_fns, "completion_fn", CompletionFnSpec)
 
-    def get_eval(self, name: str) -> EvalSpec:
+    def get_eval(self, name: str) -> Optional[EvalSpec]:
         return self._dereference(name, self._evals, "eval", EvalSpec)
 
-    def get_eval_set(self, name: str) -> EvalSetSpec:
+    def get_eval_set(self, name: str) -> Optional[EvalSetSpec]:
         return self._dereference(name, self._eval_sets, "eval set", EvalSetSpec)
 
-    def get_evals(self, patterns: Sequence[str]) -> Iterator[EvalSpec]:
+    def get_evals(self, patterns: Sequence[str]) -> Iterator[Optional[EvalSpec]]:
         # valid patterns: hello, hello.dev*, hello.dev.*-v1
-        def get_regexp(pattern):
+        def get_regexp(pattern: str) -> re.Pattern[str]:
             pattern = pattern.replace(".", "\\.")
             pattern = pattern.replace("*", ".*")
             return re.compile(f"^{pattern}$")
 
         regexps = list(map(get_regexp, patterns))
         for name in self._evals:
             # if any regexps match, return the name
             if any(map(lambda regexp: regexp.match(name), regexps)):
                 yield self.get_eval(name)
 
-    def get_base_evals(self) -> list[BaseEvalSpec]:
-        base_evals = []
+    def get_base_evals(self) -> list[Optional[BaseEvalSpec]]:
+        base_evals: list[Optional[BaseEvalSpec]] = []
         for name, spec in self._evals.items():
             if name.count(".") == 0:
                 base_evals.append(self.get_base_eval(name))
         return base_evals
 
-    def get_base_eval(self, name: str) -> BaseEvalSpec:
+    def get_base_eval(self, name: str) -> Optional[BaseEvalSpec]:
         if not name in self._evals:
             return None
 
         spec_or_alias = self._evals[name]
         if isinstance(spec_or_alias, dict):
             spec = spec_or_alias
             try:
                 return BaseEvalSpec(**spec)
             except TypeError as e:
                 raise TypeError(f"Error while processing base eval {name}: {e}")
 
         alias = spec_or_alias
         return BaseEvalSpec(id=alias)
 
-    def _process_file(self, registry, path):
+    def _process_file(self, registry: RawRegistry, path: Path) -> None:
         with open(path, "r", encoding="utf-8") as f:
             d = yaml.safe_load(f)
 
-        if d is None:
+        if d is None or not isinstance(d, dict):
             # no entries in the file
             return
 
         for name, spec in d.items():
             assert name not in registry, f"duplicate entry: {name} from {path}"
             if isinstance(spec, dict):
                 if "key" in spec:
@@ -231,45 +243,45 @@
                 spec["key"] = name
                 spec["group"] = str(os.path.basename(path).split(".")[0])
                 if "class" in spec:
                     spec["cls"] = spec["class"]
                     del spec["class"]
             registry[name] = spec
 
-    def _process_directory(self, registry, path):
+    def _process_directory(self, registry: RawRegistry, path: Path) -> None:
         files = Path(path).glob("*.yaml")
         for file in files:
             self._process_file(registry, file)
 
-    def _load_registry(self, paths):
+    def _load_registry(self, paths: Sequence[Path]) -> RawRegistry:
         """Load registry from a list of paths.
 
         Each path or yaml specifies a dictionary of name -> spec.
         """
-        registry = {}
+        registry: RawRegistry = {}
         for path in paths:
             logging.info(f"Loading registry from {path}")
             if os.path.exists(path):
                 if os.path.isdir(path):
                     self._process_directory(registry, path)
                 else:
                     self._process_file(registry, path)
         return registry
 
     @functools.cached_property
-    def _completion_fns(self):
+    def _completion_fns(self) -> RawRegistry:
         return self._load_registry([p / "completion_fns" for p in self._registry_paths])
 
     @functools.cached_property
-    def _eval_sets(self):
+    def _eval_sets(self) -> RawRegistry:
         return self._load_registry([p / "eval_sets" for p in self._registry_paths])
 
     @functools.cached_property
-    def _evals(self):
+    def _evals(self) -> RawRegistry:
         return self._load_registry([p / "evals" for p in self._registry_paths])
 
     @functools.cached_property
-    def _modelgraded_specs(self):
+    def _modelgraded_specs(self) -> RawRegistry:
         return self._load_registry([p / "modelgraded" for p in self._registry_paths])
 
 
 registry = Registry()
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/utils/api_utils.py` & `evals-nightly-1.0.3.dev20230613/evals/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals/utils/misc.py` & `evals-nightly-1.0.3.dev20230613/evals/utils/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,14 @@
         return f"{(1000*duration):0.3f}ms"
     elif duration < 60:
         return f"{duration:0.3f}s"
     else:
         return f"{duration//60}min{int(duration%60)}s"
 
 
-def make_object(object_ref: Any, *args: Any, **kwargs: Any) -> Any:
+def make_object(object_ref: str, *args: Any, **kwargs: Any) -> Any:
     modname, qualname_separator, qualname = object_ref.partition(":")
     obj = importlib.import_module(modname)
     if qualname_separator:
         for attr in qualname.split("."):
             obj = getattr(obj, attr)
     return functools.partial(obj, *args, **kwargs)
```

### Comparing `evals-nightly-1.0.3.dev20230530/evals/utils/snowflake.py` & `evals-nightly-1.0.3.dev20230613/evals/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/SOURCES.txt` & `evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,78 +15,111 @@
 evals/cli/oaievalset.py
 evals/completion_fns/__init__.py
 evals/completion_fns/cot.py
 evals/completion_fns/langchain_llm.py
 evals/completion_fns/langchain_math.py
 evals/completion_fns/openai.py
 evals/completion_fns/retrieval.py
+evals/elsuite/lambada.py
 evals/elsuite/multiple_choice.py
 evals/elsuite/translate.py
 evals/elsuite/utils.py
 evals/elsuite/utils_test.py
 evals/elsuite/basic/fuzzy_match.py
 evals/elsuite/basic/fuzzy_match_test.py
 evals/elsuite/basic/includes.py
+evals/elsuite/basic/includes_test.py
 evals/elsuite/basic/json_validator.py
+evals/elsuite/basic/json_validator_test.py
 evals/elsuite/basic/match.py
+evals/elsuite/basic/match_test.py
 evals/elsuite/modelgraded/base.py
 evals/elsuite/modelgraded/classify.py
 evals/elsuite/modelgraded/classify_utils.py
 evals/elsuite/test/match.py
 evals/prompt/base.py
 evals/registry/completion_fns/cot.yaml
 evals/registry/completion_fns/langchain_chains.yaml
 evals/registry/completion_fns/langchain_llms.yaml
 evals/registry/eval_sets/coqa-ex.yaml
+evals/registry/eval_sets/logiqa-logical-reasoning-plus.yaml
 evals/registry/eval_sets/manga-translation.yaml
+evals/registry/eval_sets/pointer-value-retrieval.yaml
+evals/registry/eval_sets/raven-matrices.yaml
 evals/registry/eval_sets/stock-options.yaml
 evals/registry/eval_sets/test-all.yaml
 evals/registry/eval_sets/test-basic.yaml
 evals/registry/eval_sets/test-modelgraded.yaml
+evals/registry/eval_sets/ukraine-gec.yaml
 evals/registry/evals/2d_movement.yaml
+evals/registry/evals/3d_globe_movement.yaml
 evals/registry/evals/aba-mrpc-true-false.yaml
+evals/registry/evals/abstract-causal-reasoning.yaml
 evals/registry/evals/actors-sequence.yaml
 evals/registry/evals/adultery_state_laws.yaml
 evals/registry/evals/afrikaans-lexicon.yaml
 evals/registry/evals/aime_evaluation.yaml
 evals/registry/evals/algebra-word-problems.yaml
+evals/registry/evals/allergen-information.yaml
+evals/registry/evals/alternate-numeral-systems.yaml
 evals/registry/evals/ambiguous-sentences.yaml
 evals/registry/evals/anagrams.yaml
+evals/registry/evals/arc.yaml
 evals/registry/evals/arithmetical_puzzles.yaml
 evals/registry/evals/ascii-wordart.yaml
+evals/registry/evals/asl-classifiers.yaml
 evals/registry/evals/atpl_exams.yaml
 evals/registry/evals/balance-chemical-equation.yaml
 evals/registry/evals/banking77.yaml
+evals/registry/evals/beam-analysis.yaml
+evals/registry/evals/belarusian-grammar.yaml
 evals/registry/evals/belarusian-lexicon.yaml
+evals/registry/evals/belarusian-proverbs.yaml
+evals/registry/evals/belarusian-russian-translation.yaml
+evals/registry/evals/belarusian-syllable-count.yaml
+evals/registry/evals/belarusian-synonyms.yaml
 evals/registry/evals/bigrams.yaml
 evals/registry/evals/bitwise.yaml
 evals/registry/evals/body-movement.yaml
 evals/registry/evals/born-first.yaml
 evals/registry/evals/brazilian-lexicon.yaml
+evals/registry/evals/brazilian_laws.yaml
 evals/registry/evals/building_floorplan.yaml
 evals/registry/evals/bulgarian-lexicon.yaml
+evals/registry/evals/canto_wu_pronunciation.yaml
+evals/registry/evals/canto_wu_pronunciation_fewshot.yaml
+evals/registry/evals/cardinal-directions.yaml
 evals/registry/evals/categorize_with_distractors.yaml
 evals/registry/evals/chess-piece-count.yaml
 evals/registry/evals/chess.yaml
+evals/registry/evals/chinese_homonym.yaml
 evals/registry/evals/chinese_poem.yaml
+evals/registry/evals/chinese_song_ci.yaml
 evals/registry/evals/chinese_tang_poetries.yaml
+evals/registry/evals/chinese_zodiac.yaml
 evals/registry/evals/cissp-study-questions.yaml
+evals/registry/evals/code_combination.yaml
 evals/registry/evals/color_theory_complementary.yaml
 evals/registry/evals/compare-countries-area.yaml
+evals/registry/evals/complex-analogies-en-ru.yaml
 evals/registry/evals/complex-replace-characters.yaml
+evals/registry/evals/comprehensive-graph-reasoning.yaml
 evals/registry/evals/connect-4.yaml
+evals/registry/evals/context-free-grammar.yaml
 evals/registry/evals/convert-hex-hsl-lightness.yaml
 evals/registry/evals/coqa-ex.yaml
 evals/registry/evals/count_intersections_polynomial.yaml
 evals/registry/evals/count_token_freq_dna.yaml
 evals/registry/evals/counterfactual-reasoning.yaml
 evals/registry/evals/countries.yaml
 evals/registry/evals/crepe.yaml
+evals/registry/evals/cricket_situations.yaml
 evals/registry/evals/crontab.yaml
 evals/registry/evals/cube-pack.yaml
+evals/registry/evals/cybersecurity-filepaths.yaml
 evals/registry/evals/date-booking.yaml
 evals/registry/evals/date-calculator.yaml
 evals/registry/evals/day-of-week-from-date.yaml
 evals/registry/evals/decrypt-caesar-cipher.yaml
 evals/registry/evals/detect-hshd.yaml
 evals/registry/evals/determinant.yaml
 evals/registry/evals/diabetes.yaml
@@ -95,163 +128,230 @@
 evals/registry/evals/direct-speech-tag.yaml
 evals/registry/evals/directions.yaml
 evals/registry/evals/dna-melting-calculation.yaml
 evals/registry/evals/dutch-lexicon.yaml
 evals/registry/evals/emoji-riddle.yaml
 evals/registry/evals/emotional-intelligence.yaml
 evals/registry/evals/escher-sentences.yaml
+evals/registry/evals/euler_problems.yaml
 evals/registry/evals/european-date-format-challenge.yaml
 evals/registry/evals/event-categories.yaml
 evals/registry/evals/fcc_amateur_extra.yaml
 evals/registry/evals/finance.yaml
 evals/registry/evals/financial-derivatives.yaml
 evals/registry/evals/find-letter.yaml
 evals/registry/evals/find-thirukkural.yaml
 evals/registry/evals/find_country_from_svg.yaml
 evals/registry/evals/finnish-rhyme.yaml
 evals/registry/evals/first-letters.yaml
 evals/registry/evals/food.yaml
+evals/registry/evals/formal-grammar-to-regex.yaml
 evals/registry/evals/formal_logic.yaml
 evals/registry/evals/forth-stack-sim.yaml
 evals/registry/evals/french-lexicon.yaml
 evals/registry/evals/french-part-of-speech.yaml
+evals/registry/evals/game-theory.yaml
+evals/registry/evals/geometry_puzzle.yaml
+evals/registry/evals/german-part-of-speech.yaml
 evals/registry/evals/gol.yaml
+evals/registry/evals/gpt-protocol-buffers.yaml
+evals/registry/evals/greek-nt-manuscripts.yaml
 evals/registry/evals/greek-vocabulary.yaml
 evals/registry/evals/guess-the-singer.yaml
 evals/registry/evals/heart-disease.yaml
+evals/registry/evals/hebrew-bible.yaml
 evals/registry/evals/hebrew-rhyme.yaml
 evals/registry/evals/hebrew-same-noun-gender.yaml
 evals/registry/evals/hindi_shuddha.yaml
 evals/registry/evals/hindi_upsc.yaml
 evals/registry/evals/hindi_words.yaml
+evals/registry/evals/historical-kana-orthography-reading.yaml
+evals/registry/evals/human-safety.yaml
+evals/registry/evals/iambic-pentameter.yaml
 evals/registry/evals/illinois-law.yaml
 evals/registry/evals/imperial_date_to_string.yaml
+evals/registry/evals/indonesian_numbers.yaml
 evals/registry/evals/infiniteloop-match.yaml
 evals/registry/evals/integer-sequence-predictions.yaml
 evals/registry/evals/internal_representations.yaml
 evals/registry/evals/invert_word_wise.yaml
 evals/registry/evals/invoice_due_date_leap_day_adjustment.yaml
 evals/registry/evals/invoices.yaml
 evals/registry/evals/irish-lexicon.yaml
 evals/registry/evals/irony.yaml
 evals/registry/evals/islands.yaml
 evals/registry/evals/isosceles-right-triangle.yaml
 evals/registry/evals/italian-new-words.yaml
 evals/registry/evals/italian-rhyme.yaml
 evals/registry/evals/japanese-itpassport-exam01.yaml
 evals/registry/evals/japanese-national-medical-exam01.yaml
+evals/registry/evals/japanese-national-medical-exam02.yaml
 evals/registry/evals/japanese_city_name_pronuciation.yaml
 evals/registry/evals/japanese_driving_license.yaml
 evals/registry/evals/japanese_number_reading.yaml
 evals/registry/evals/japanese_populer_video_game_title_and_the_publisher.yaml
 evals/registry/evals/jee-math.yaml
 evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
+evals/registry/evals/json_patch_object.yaml
 evals/registry/evals/kanji-idioms.yaml
 evals/registry/evals/knot-theory.yaml
 evals/registry/evals/korean-consonant-vowel-combination.yaml
+evals/registry/evals/korean-phonetics.yaml
+evals/registry/evals/korean_dialects.yaml
 evals/registry/evals/korean_spelling.yaml
+evals/registry/evals/korean_yaminjeongeum.yaml
 evals/registry/evals/language.yaml
 evals/registry/evals/largest_country.yaml
 evals/registry/evals/last-word-nth.yaml
 evals/registry/evals/lat_long_identify.yaml
 evals/registry/evals/linear-equations.yaml
 evals/registry/evals/linear-regression.yaml
 evals/registry/evals/list_comparison_missing_name.yaml
+evals/registry/evals/logic-grid-eval.yaml
 evals/registry/evals/logic-liar-paradox.yaml
+evals/registry/evals/logic-riddles.yaml
 evals/registry/evals/logic-statements.yaml
 evals/registry/evals/logic.yaml
+evals/registry/evals/logic_and_probability.yaml
 evals/registry/evals/logical_counting.yaml
+evals/registry/evals/logiqa-logical-reasoning-plus.yaml
 evals/registry/evals/logiqa.yaml
 evals/registry/evals/loss-logic.yaml
 evals/registry/evals/lunar-calendar.yaml
 evals/registry/evals/mandaliof-table.yaml
 evals/registry/evals/manga-translation.yaml
 evals/registry/evals/map-electronic-component-part-to-fact.yaml
+evals/registry/evals/mapping_to_matricies.yaml
 evals/registry/evals/mate-in-one.yaml
 evals/registry/evals/matrix-mult-rows.yaml
+evals/registry/evals/medication_dose.yaml
 evals/registry/evals/medmcqa.yaml
 evals/registry/evals/mendelian_inheritance.yaml
 evals/registry/evals/missing-operators.yaml
 evals/registry/evals/mmlu.yaml
+evals/registry/evals/monthly_metric_comparison.yaml
 evals/registry/evals/moral_exceptQA.yaml
 evals/registry/evals/multi-step-equations.yaml
 evals/registry/evals/multistep-word-problems.yaml
 evals/registry/evals/music-theory-chord-names.yaml
 evals/registry/evals/music-theory-chord-notes.yaml
+evals/registry/evals/music-theory.yaml
 evals/registry/evals/music_theory_scale_modes.yaml
 evals/registry/evals/naughty_strings.yaml
 evals/registry/evals/nepali-song-singer.yaml
 evals/registry/evals/newsology.yaml
+evals/registry/evals/next-val-series.yaml
+evals/registry/evals/nfl-point-combinations.yaml
+evals/registry/evals/non-compound-names.yaml
 evals/registry/evals/norwegian-lexicon.yaml
 evals/registry/evals/number-pattern.yaml
 evals/registry/evals/number-reading.yaml
 evals/registry/evals/numbers_game.yaml
+evals/registry/evals/numeral-type-comparisons.yaml
 evals/registry/evals/nutrition.yaml
 evals/registry/evals/ordered-history-events.yaml
+evals/registry/evals/override-system-instruction.yaml
+evals/registry/evals/pantone_to_hex.yaml
+evals/registry/evals/parable-to-moral-match.yaml
 evals/registry/evals/pararule-plus-multi-step-deductive-reasoning.yaml
 evals/registry/evals/partially_solved_crossword_clues.yaml
+evals/registry/evals/passing-balls.yaml
 evals/registry/evals/pattern_identification.yaml
 evals/registry/evals/ph_calculation.yaml
+evals/registry/evals/phonetics-identify-words-needing-missing-gpcs.yaml
 evals/registry/evals/physics-interaction.yaml
+evals/registry/evals/pointer-value-retrieval.yaml
+evals/registry/evals/points-on-line.yaml
+evals/registry/evals/poker_analysis.yaml
 evals/registry/evals/poker_hand_ranks.yaml
+evals/registry/evals/polish-lexicon.yaml
+evals/registry/evals/polish-syllable-count.yaml
 evals/registry/evals/polish_rhymes_generation.yaml
+evals/registry/evals/population_span_extraction.yaml
 evals/registry/evals/portuguese-sarcasm.yaml
 evals/registry/evals/portuguese-syllable-count.yaml
 evals/registry/evals/positive-binary-operations.yaml
 evals/registry/evals/probability_questions.yaml
+evals/registry/evals/product-matching.yaml
+evals/registry/evals/prompt-injection.yaml
+evals/registry/evals/pure_korean.yaml
 evals/registry/evals/python_list_comprehension.yaml
 evals/registry/evals/qa.yaml
+evals/registry/evals/quartz.yaml
+evals/registry/evals/rare-and-loanwords-dutch-lexicon.yaml
+evals/registry/evals/raven-matrices.yaml
+evals/registry/evals/rectangles.yaml
 evals/registry/evals/regex-match.yaml
 evals/registry/evals/resistor-ohm-calculator.yaml
+evals/registry/evals/resource_id_extraction.yaml
 evals/registry/evals/reverse-polish-notation.yaml
+evals/registry/evals/reverse-sort-words-eng.yaml
 evals/registry/evals/reverse-string.yaml
 evals/registry/evals/rhetorical-devices.yaml
+evals/registry/evals/rock-climbing.yaml
 evals/registry/evals/rot13.yaml
+evals/registry/evals/ru_rhymes.yaml
 evals/registry/evals/rubiks-colors.yaml
 evals/registry/evals/rucola.yaml
 evals/registry/evals/russe.yaml
+evals/registry/evals/russian-english-homonym-context-resolution.yaml
 evals/registry/evals/russian-lexicon.yaml
 evals/registry/evals/russian-nlp-tasks.yaml
 evals/registry/evals/russian-rhyme.yaml
+evals/registry/evals/russian-verse.yaml
 evals/registry/evals/russian_medical.yaml
+evals/registry/evals/russian_sarcasm.yaml
 evals/registry/evals/sarcasm.yaml
 evals/registry/evals/seating_arrangements.yaml
 evals/registry/evals/security_guide.yaml
 evals/registry/evals/sexagenary-cycle-calculation.yaml
 evals/registry/evals/shape-in-shape.yaml
 evals/registry/evals/shared-borders.yaml
+evals/registry/evals/shopping_discount_comparison.yaml
 evals/registry/evals/simple-knowledge-mongolian.yaml
 evals/registry/evals/simple-visual-understanding.yaml
+evals/registry/evals/simple_math.yaml
+evals/registry/evals/simple_physics_engine.yaml
+evals/registry/evals/sindarin-fluency.yaml
+evals/registry/evals/soc_codes.yaml
+evals/registry/evals/solve-for-variable.yaml
 evals/registry/evals/sort-numeric.yaml
 evals/registry/evals/south-african-bands.yaml
 evals/registry/evals/spanish-lexicon.yaml
 evals/registry/evals/spanish_feminine_noun_masculine_article.yaml
+evals/registry/evals/split_chinese_characters.yaml
 evals/registry/evals/sql.yaml
 evals/registry/evals/squares-gpt.yaml
+evals/registry/evals/stats-tests.yaml
 evals/registry/evals/stock-options.yaml
 evals/registry/evals/superficial-patterns.yaml
 evals/registry/evals/svg_understanding.yaml
 evals/registry/evals/swap-words.yaml
 evals/registry/evals/swedish-spelling.yaml
 evals/registry/evals/swedish_sat.yaml
+evals/registry/evals/syllables_long_words.yaml
 evals/registry/evals/syntax-check.yaml
 evals/registry/evals/taxes.yaml
 evals/registry/evals/tempo_to_measure_count.yaml
 evals/registry/evals/test-basic.yaml
 evals/registry/evals/test-comp-sci.yaml
 evals/registry/evals/test-modelgraded-battle.yaml
 evals/registry/evals/test-modelgraded-generated.yaml
 evals/registry/evals/test-modelgraded.yaml
+evals/registry/evals/test_japanese_radical.yaml
 evals/registry/evals/test_japanese_units.yaml
 evals/registry/evals/tetris.yaml
 evals/registry/evals/three-pt-mapping.yaml
 evals/registry/evals/time-zone-conversion.yaml
 evals/registry/evals/track_objects.yaml
 evals/registry/evals/tracking-shuffled-objects.yaml
+evals/registry/evals/turkish_characters.yaml
 evals/registry/evals/ukraine-eit.yaml
+evals/registry/evals/ukraine-gec.yaml
+evals/registry/evals/ukraine_electronic_petitions.yaml
 evals/registry/evals/unified-patch.yaml
 evals/registry/evals/unique_combinations.yaml
 evals/registry/evals/unsolvable_questions.yaml
 evals/registry/evals/unwanted-rhyming.yaml
 evals/registry/evals/us-tort-law.yaml
 evals/registry/evals/utility_price_parsing.yaml
 evals/registry/evals/vigenere.yaml
@@ -261,20 +361,22 @@
 evals/registry/evals/word_vector_over_reliance.yaml
 evals/registry/modelgraded/battle.yaml
 evals/registry/modelgraded/best.yaml
 evals/registry/modelgraded/closedqa.yaml
 evals/registry/modelgraded/diversity.yaml
 evals/registry/modelgraded/fact.yaml
 evals/registry/modelgraded/humor.yaml
+evals/registry/modelgraded/iambic_pentameter.yaml
 evals/registry/modelgraded/regression-equation.yaml
 evals/registry/modelgraded/rhyming.yaml
 evals/registry/modelgraded/security.yaml
 evals/registry/modelgraded/sql.yaml
 evals/utils/api_utils.py
 evals/utils/misc.py
 evals/utils/snowflake.py
+evals/utils/test.py
 evals_nightly.egg-info/PKG-INFO
 evals_nightly.egg-info/SOURCES.txt
 evals_nightly.egg-info/dependency_links.txt
 evals_nightly.egg-info/entry_points.txt
 evals_nightly.egg-info/requires.txt
 evals_nightly.egg-info/top_level.txt
```

