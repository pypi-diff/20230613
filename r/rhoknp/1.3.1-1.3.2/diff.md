# Comparing `tmp/rhoknp-1.3.1.tar.gz` & `tmp/rhoknp-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhoknp-1.3.1.tar", max compression
+gzip compressed data, was "rhoknp-1.3.2.tar", max compression
```

## Comparing `rhoknp-1.3.1.tar` & `rhoknp-1.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1073 2022-07-07 05:13:45.612050 rhoknp-1.3.1/LICENSE
--rw-r--r--   0        0        0     6528 2023-06-01 10:08:32.507270 rhoknp-1.3.1/README.md
--rw-r--r--   0        0        0     1849 2023-06-01 10:08:39.510243 rhoknp-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      474 2023-01-23 11:06:01.235960 rhoknp-1.3.1/src/rhoknp/__init__.py
--rw-r--r--   0        0        0      293 2023-01-25 04:22:29.044533 rhoknp-1.3.1/src/rhoknp/cli/__init__.py
--rw-r--r--   0        0        0     3334 2023-05-01 10:39:22.239944 rhoknp-1.3.1/src/rhoknp/cli/cli.py
--rw-r--r--   0        0        0     6802 2023-05-01 10:39:22.240180 rhoknp-1.3.1/src/rhoknp/cli/serve.py
--rw-r--r--   0        0        0     5782 2023-05-01 10:39:22.240529 rhoknp-1.3.1/src/rhoknp/cli/show.py
--rw-r--r--   0        0        0      823 2023-05-01 10:39:22.240711 rhoknp-1.3.1/src/rhoknp/cli/static/css/style.css
--rw-r--r--   0        0        0     9898 2023-05-01 10:39:22.241416 rhoknp-1.3.1/src/rhoknp/cli/static/images/apple-touch-icon.png
--rw-r--r--   0        0        0    15086 2023-05-01 10:39:22.242054 rhoknp-1.3.1/src/rhoknp/cli/static/images/favicon.ico
--rw-r--r--   0        0        0     1960 2023-05-01 10:39:22.242198 rhoknp-1.3.1/src/rhoknp/cli/static/js/script.js
--rw-r--r--   0        0        0     1779 2023-01-23 11:06:01.236808 rhoknp-1.3.1/src/rhoknp/cli/stats.py
--rw-r--r--   0        0        0     1705 2023-05-01 10:39:22.242748 rhoknp-1.3.1/src/rhoknp/cli/templates/base.jinja2
--rw-r--r--   0        0        0      724 2023-05-01 10:39:22.242904 rhoknp-1.3.1/src/rhoknp/cli/templates/components/dependency_parsing.jinja2
--rw-r--r--   0        0        0     1840 2023-05-01 10:39:22.243108 rhoknp-1.3.1/src/rhoknp/cli/templates/components/discourse_parsing.jinja2
--rw-r--r--   0        0        0      276 2023-05-01 10:39:22.243247 rhoknp-1.3.1/src/rhoknp/cli/templates/components/error.jinja2
--rw-r--r--   0        0        0      344 2023-05-01 10:39:22.243341 rhoknp-1.3.1/src/rhoknp/cli/templates/components/form.jinja2
--rw-r--r--   0        0        0      136 2023-05-01 10:39:22.243485 rhoknp-1.3.1/src/rhoknp/cli/templates/components/hide_all_button.jinja2
--rw-r--r--   0        0        0     1987 2023-05-01 10:39:22.243568 rhoknp-1.3.1/src/rhoknp/cli/templates/components/morphological_analysis.jinja2
--rw-r--r--   0        0        0     1063 2023-05-01 10:39:22.243719 rhoknp-1.3.1/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2
--rw-r--r--   0        0        0      163 2023-05-01 10:39:22.243791 rhoknp-1.3.1/src/rhoknp/cli/templates/components/navbar.jinja2
--rw-r--r--   0        0        0       63 2023-05-01 10:39:22.244032 rhoknp-1.3.1/src/rhoknp/cli/templates/components/raw_input.jinja2
--rw-r--r--   0        0        0      636 2023-05-01 10:39:22.244218 rhoknp-1.3.1/src/rhoknp/cli/templates/components/raw_output.jinja2
--rw-r--r--   0        0        0      131 2023-05-01 10:39:22.244412 rhoknp-1.3.1/src/rhoknp/cli/templates/components/show_all_button.jinja2
--rw-r--r--   0        0        0     1034 2023-05-01 10:39:22.244575 rhoknp-1.3.1/src/rhoknp/cli/templates/components/typo_correction.jinja2
--rw-r--r--   0        0        0      722 2023-05-01 10:39:22.244665 rhoknp-1.3.1/src/rhoknp/cli/templates/components/word_splitting.jinja2
--rw-r--r--   0        0        0      333 2023-05-01 10:39:22.244808 rhoknp-1.3.1/src/rhoknp/cli/templates/jumanpp.jinja2
--rw-r--r--   0        0        0      526 2023-05-01 10:39:22.244946 rhoknp-1.3.1/src/rhoknp/cli/templates/knp.jinja2
--rw-r--r--   0        0        0      643 2023-05-01 10:39:22.245089 rhoknp-1.3.1/src/rhoknp/cli/templates/kwja.jinja2
--rw-r--r--   0        0        0      826 2023-01-23 11:06:01.237203 rhoknp-1.3.1/src/rhoknp/cohesion/__init__.py
--rw-r--r--   0        0        0     6744 2023-02-07 06:49:22.772304 rhoknp-1.3.1/src/rhoknp/cohesion/argument.py
--rw-r--r--   0        0        0     9899 2023-02-07 06:49:22.772615 rhoknp-1.3.1/src/rhoknp/cohesion/coreference.py
--rw-r--r--   0        0        0     9566 2023-01-23 11:06:01.238718 rhoknp-1.3.1/src/rhoknp/cohesion/discourse.py
--rw-r--r--   0        0        0     2427 2023-01-23 11:06:01.239467 rhoknp-1.3.1/src/rhoknp/cohesion/exophora.py
--rw-r--r--   0        0        0    10329 2023-02-07 06:49:22.772957 rhoknp-1.3.1/src/rhoknp/cohesion/pas.py
--rw-r--r--   0        0        0     2595 2023-01-23 11:06:01.239969 rhoknp-1.3.1/src/rhoknp/cohesion/predicate.py
--rw-r--r--   0        0        0     4716 2023-01-23 11:06:01.240472 rhoknp-1.3.1/src/rhoknp/cohesion/rel.py
--rw-r--r--   0        0        0      226 2023-01-23 11:06:01.240680 rhoknp-1.3.1/src/rhoknp/processors/__init__.py
--rw-r--r--   0        0        0     5264 2023-05-01 10:39:22.245299 rhoknp-1.3.1/src/rhoknp/processors/jumanpp.py
--rw-r--r--   0        0        0     7027 2023-05-01 10:39:22.245466 rhoknp-1.3.1/src/rhoknp/processors/knp.py
--rw-r--r--   0        0        0     5617 2023-05-01 10:39:22.245819 rhoknp-1.3.1/src/rhoknp/processors/kwja.py
--rw-r--r--   0        0        0     2984 2022-10-29 15:30:49.159597 rhoknp-1.3.1/src/rhoknp/processors/processor.py
--rw-r--r--   0        0        0     3070 2023-05-01 10:39:22.245994 rhoknp-1.3.1/src/rhoknp/processors/senter.py
--rw-r--r--   0        0        0      378 2023-01-23 11:06:01.241792 rhoknp-1.3.1/src/rhoknp/props/__init__.py
--rw-r--r--   0        0        0      210 2022-10-24 08:19:10.843963 rhoknp-1.3.1/src/rhoknp/props/dependency.py
--rw-r--r--   0        0        0     1996 2023-01-23 11:06:01.242202 rhoknp-1.3.1/src/rhoknp/props/feature.py
--rw-r--r--   0        0        0      863 2023-01-23 11:06:01.242583 rhoknp-1.3.1/src/rhoknp/props/memo.py
--rw-r--r--   0        0        0     2917 2023-02-07 06:49:22.773596 rhoknp-1.3.1/src/rhoknp/props/named_entity.py
--rw-r--r--   0        0        0     1633 2023-01-23 11:06:01.243129 rhoknp-1.3.1/src/rhoknp/props/semantics.py
--rw-r--r--   0        0        0        0 2022-07-07 07:10:30.837345 rhoknp-1.3.1/src/rhoknp/py.typed
--rw-r--r--   0        0        0      337 2023-01-23 11:06:01.243840 rhoknp-1.3.1/src/rhoknp/units/__init__.py
--rw-r--r--   0        0        0    14479 2023-03-03 06:23:17.602965 rhoknp-1.3.1/src/rhoknp/units/base_phrase.py
--rw-r--r--   0        0        0     7740 2023-02-07 06:49:22.774401 rhoknp-1.3.1/src/rhoknp/units/clause.py
--rw-r--r--   0        0        0    15809 2023-02-07 06:49:22.774863 rhoknp-1.3.1/src/rhoknp/units/document.py
--rw-r--r--   0        0        0    12324 2023-06-01 10:08:39.510621 rhoknp-1.3.1/src/rhoknp/units/morpheme.py
--rw-r--r--   0        0        0     7202 2023-02-07 06:49:22.775468 rhoknp-1.3.1/src/rhoknp/units/phrase.py
--rw-r--r--   0        0        0    18039 2023-05-01 10:39:22.246566 rhoknp-1.3.1/src/rhoknp/units/sentence.py
--rw-r--r--   0        0        0     1521 2023-01-23 11:06:01.246571 rhoknp-1.3.1/src/rhoknp/units/unit.py
--rw-r--r--   0        0        0        0 2023-01-23 11:06:01.246629 rhoknp-1.3.1/src/rhoknp/utils/__init__.py
--rw-r--r--   0        0        0     3783 2023-05-01 10:39:22.247129 rhoknp-1.3.1/src/rhoknp/utils/reader.py
--rw-r--r--   0        0        0     1112 2023-05-01 10:39:22.247398 rhoknp-1.3.1/src/rhoknp/utils/util.py
--rw-r--r--   0        0        0     7888 1970-01-01 00:00:00.000000 rhoknp-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-10 08:06:05.999782 rhoknp-1.3.2/LICENSE
+-rw-r--r--   0        0        0     6740 2023-06-13 05:50:36.170332 rhoknp-1.3.2/README.md
+-rw-r--r--   0        0        0     1849 2023-06-13 05:50:36.171714 rhoknp-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-10 08:06:06.005858 rhoknp-1.3.2/src/rhoknp/__init__.py
+-rw-r--r--   0        0        0      293 2023-04-10 08:06:06.005941 rhoknp-1.3.2/src/rhoknp/cli/__init__.py
+-rw-r--r--   0        0        0     3465 2023-06-13 05:50:36.172071 rhoknp-1.3.2/src/rhoknp/cli/cli.py
+-rw-r--r--   0        0        0     6811 2023-06-13 05:50:36.172410 rhoknp-1.3.2/src/rhoknp/cli/serve.py
+-rw-r--r--   0        0        0     5782 2023-05-19 02:08:59.237964 rhoknp-1.3.2/src/rhoknp/cli/show.py
+-rw-r--r--   0        0        0      798 2023-06-13 05:50:36.172747 rhoknp-1.3.2/src/rhoknp/cli/static/css/style.css
+-rw-r--r--   0        0        0     9898 2023-05-08 05:46:59.165389 rhoknp-1.3.2/src/rhoknp/cli/static/images/apple-touch-icon.png
+-rw-r--r--   0        0        0    15086 2023-05-08 05:46:59.165659 rhoknp-1.3.2/src/rhoknp/cli/static/images/favicon.ico
+-rw-r--r--   0        0        0     1961 2023-06-13 05:50:36.173052 rhoknp-1.3.2/src/rhoknp/cli/static/js/script.js
+-rw-r--r--   0        0        0     1779 2023-04-10 08:06:06.006221 rhoknp-1.3.2/src/rhoknp/cli/stats.py
+-rw-r--r--   0        0        0     1738 2023-06-13 05:50:36.173385 rhoknp-1.3.2/src/rhoknp/cli/templates/base.jinja2
+-rw-r--r--   0        0        0      724 2023-05-08 05:46:59.166545 rhoknp-1.3.2/src/rhoknp/cli/templates/components/dependency_parsing.jinja2
+-rw-r--r--   0        0        0     1840 2023-05-08 05:46:59.166810 rhoknp-1.3.2/src/rhoknp/cli/templates/components/discourse_parsing.jinja2
+-rw-r--r--   0        0        0      276 2023-05-08 05:46:59.167058 rhoknp-1.3.2/src/rhoknp/cli/templates/components/error.jinja2
+-rw-r--r--   0        0        0      344 2023-05-08 05:46:59.167151 rhoknp-1.3.2/src/rhoknp/cli/templates/components/form.jinja2
+-rw-r--r--   0        0        0      136 2023-05-08 05:46:59.167337 rhoknp-1.3.2/src/rhoknp/cli/templates/components/hide_all_button.jinja2
+-rw-r--r--   0        0        0     1987 2023-05-08 05:46:59.167591 rhoknp-1.3.2/src/rhoknp/cli/templates/components/morphological_analysis.jinja2
+-rw-r--r--   0        0        0     1063 2023-05-08 05:46:59.167781 rhoknp-1.3.2/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2
+-rw-r--r--   0        0        0      176 2023-06-13 05:50:36.173712 rhoknp-1.3.2/src/rhoknp/cli/templates/components/navbar.jinja2
+-rw-r--r--   0        0        0       63 2023-05-08 05:46:59.167915 rhoknp-1.3.2/src/rhoknp/cli/templates/components/raw_input.jinja2
+-rw-r--r--   0        0        0      636 2023-05-08 05:46:59.168164 rhoknp-1.3.2/src/rhoknp/cli/templates/components/raw_output.jinja2
+-rw-r--r--   0        0        0      131 2023-05-08 05:46:59.168361 rhoknp-1.3.2/src/rhoknp/cli/templates/components/show_all_button.jinja2
+-rw-r--r--   0        0        0     1034 2023-05-08 05:46:59.168493 rhoknp-1.3.2/src/rhoknp/cli/templates/components/typo_correction.jinja2
+-rw-r--r--   0        0        0      722 2023-05-08 05:46:59.168662 rhoknp-1.3.2/src/rhoknp/cli/templates/components/word_splitting.jinja2
+-rw-r--r--   0        0        0      333 2023-05-08 05:46:59.168876 rhoknp-1.3.2/src/rhoknp/cli/templates/jumanpp.jinja2
+-rw-r--r--   0        0        0      526 2023-05-08 05:46:59.169052 rhoknp-1.3.2/src/rhoknp/cli/templates/knp.jinja2
+-rw-r--r--   0        0        0      643 2023-05-08 05:46:59.169189 rhoknp-1.3.2/src/rhoknp/cli/templates/kwja.jinja2
+-rw-r--r--   0        0        0      826 2023-04-10 08:06:06.006307 rhoknp-1.3.2/src/rhoknp/cohesion/__init__.py
+-rw-r--r--   0        0        0     6744 2023-05-19 02:08:59.238650 rhoknp-1.3.2/src/rhoknp/cohesion/argument.py
+-rw-r--r--   0        0        0     9899 2023-04-10 08:06:06.006487 rhoknp-1.3.2/src/rhoknp/cohesion/coreference.py
+-rw-r--r--   0        0        0     9566 2023-06-12 06:53:07.590307 rhoknp-1.3.2/src/rhoknp/cohesion/discourse.py
+-rw-r--r--   0        0        0     2427 2023-06-12 06:53:07.590479 rhoknp-1.3.2/src/rhoknp/cohesion/exophora.py
+-rw-r--r--   0        0        0    10329 2023-06-12 07:01:36.506728 rhoknp-1.3.2/src/rhoknp/cohesion/pas.py
+-rw-r--r--   0        0        0     2595 2023-04-10 08:06:06.006784 rhoknp-1.3.2/src/rhoknp/cohesion/predicate.py
+-rw-r--r--   0        0        0     4716 2023-06-12 07:01:36.506926 rhoknp-1.3.2/src/rhoknp/cohesion/rel.py
+-rw-r--r--   0        0        0      226 2023-04-10 08:06:06.006922 rhoknp-1.3.2/src/rhoknp/processors/__init__.py
+-rw-r--r--   0        0        0     5264 2023-06-12 06:53:07.591032 rhoknp-1.3.2/src/rhoknp/processors/jumanpp.py
+-rw-r--r--   0        0        0     7027 2023-06-12 06:53:07.591325 rhoknp-1.3.2/src/rhoknp/processors/knp.py
+-rw-r--r--   0        0        0     5617 2023-06-12 06:53:07.591517 rhoknp-1.3.2/src/rhoknp/processors/kwja.py
+-rw-r--r--   0        0        0     2984 2023-04-10 08:06:06.007166 rhoknp-1.3.2/src/rhoknp/processors/processor.py
+-rw-r--r--   0        0        0     3294 2023-06-13 05:50:36.174078 rhoknp-1.3.2/src/rhoknp/processors/senter.py
+-rw-r--r--   0        0        0      378 2023-04-10 08:06:06.007305 rhoknp-1.3.2/src/rhoknp/props/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-10 08:06:06.007355 rhoknp-1.3.2/src/rhoknp/props/dependency.py
+-rw-r--r--   0        0        0     1996 2023-04-10 08:06:06.007411 rhoknp-1.3.2/src/rhoknp/props/feature.py
+-rw-r--r--   0        0        0      863 2023-06-12 06:53:07.592074 rhoknp-1.3.2/src/rhoknp/props/memo.py
+-rw-r--r--   0        0        0     2917 2023-06-12 06:53:07.592215 rhoknp-1.3.2/src/rhoknp/props/named_entity.py
+-rw-r--r--   0        0        0     1633 2023-04-10 08:06:06.007581 rhoknp-1.3.2/src/rhoknp/props/semantics.py
+-rw-r--r--   0        0        0        0 2023-04-10 08:06:06.007602 rhoknp-1.3.2/src/rhoknp/py.typed
+-rw-r--r--   0        0        0      337 2023-04-10 08:06:06.007676 rhoknp-1.3.2/src/rhoknp/units/__init__.py
+-rw-r--r--   0        0        0    14479 2023-04-10 08:06:06.007777 rhoknp-1.3.2/src/rhoknp/units/base_phrase.py
+-rw-r--r--   0        0        0     7740 2023-04-10 08:06:06.007869 rhoknp-1.3.2/src/rhoknp/units/clause.py
+-rw-r--r--   0        0        0    15809 2023-05-01 05:28:13.915982 rhoknp-1.3.2/src/rhoknp/units/document.py
+-rw-r--r--   0        0        0    12324 2023-06-12 06:53:07.592477 rhoknp-1.3.2/src/rhoknp/units/morpheme.py
+-rw-r--r--   0        0        0     7202 2023-06-12 07:01:36.507376 rhoknp-1.3.2/src/rhoknp/units/phrase.py
+-rw-r--r--   0        0        0    18039 2023-05-08 05:46:59.170172 rhoknp-1.3.2/src/rhoknp/units/sentence.py
+-rw-r--r--   0        0        0     1521 2023-04-10 08:06:06.008284 rhoknp-1.3.2/src/rhoknp/units/unit.py
+-rw-r--r--   0        0        0        0 2023-04-10 08:06:06.008333 rhoknp-1.3.2/src/rhoknp/utils/__init__.py
+-rw-r--r--   0        0        0     3783 2023-06-12 07:01:36.507719 rhoknp-1.3.2/src/rhoknp/utils/reader.py
+-rw-r--r--   0        0        0     1112 2023-06-12 06:53:07.592960 rhoknp-1.3.2/src/rhoknp/utils/util.py
+-rw-r--r--   0        0        0     8100 1970-01-01 00:00:00.000000 rhoknp-1.3.2/PKG-INFO
```

### Comparing `rhoknp-1.3.1/LICENSE` & `rhoknp-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/README.md` & `rhoknp-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,72 +12,73 @@
 <a href="https://www.codefactor.io/repository/github/ku-nlp/rhoknp"><img alt="CodeFactor" src="https://img.shields.io/codefactor/grade/github/ku-nlp/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rhoknp?style=flat-square">
 <a href="https://rhoknp.readthedocs.io/en/latest/"><img alt="Documentation" src="https://img.shields.io/readthedocs/rhoknp?style=flat-square"></a>
 <a href="https://github.com/psf/black"><img alt="Code style - black" src="https://img.shields.io/badge/code%20style-black-222222?style=flat-square"></a>
 </p>
 
+---
+
+**Documentation**: [https://rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/)
+
+**Source Code**: [https://github.com/ku-nlp/rhoknp](https://github.com/ku-nlp/rhoknp)
+
+---
+
 _rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1]
 
-[^1]: The logo was originally generated using OpenAI DALL·E 2
+[^1]: The logo was generated by OpenAI DALL·E 2.
 
 ```python
 import rhoknp
 
-# Perform language analysis by Juman++
+# Perform morphological analysis by Juman++
 jumanpp = rhoknp.Jumanpp()
 sentence = jumanpp.apply_to_sentence(
     "電気抵抗率は電気の通しにくさを表す物性値である。"
 )
 
 # Access to the result
 for morpheme in sentence.morphemes:  # a.k.a. keitai-so
     ...
 
-# Save language analysis by Juman++
+# Save the result
 with open("result.jumanpp", "wt") as f:
     f.write(sentence.to_jumanpp())
 
-# Load language analysis by Juman++
+# Load the result
 with open("result.jumanpp", "rt") as f:
     sentence = rhoknp.Sentence.from_jumanpp(f.read())
 ```
 
 ## Requirements
 
 - Python 3.7+
-
-## Optional requirements for language analysis
-
-- [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+
-- [KNP](https://github.com/ku-nlp/knp) 5.0+
-- [KWJA](https://github.com/ku-nlp/kwja) 1.0.0+
+- (Optional) [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+
+- (Optional) [KNP](https://github.com/ku-nlp/knp) 5.0+
+- (Optional) [KWJA](https://github.com/ku-nlp/kwja) 1.0.0+
 
 ## Installation
 
 ```shell
 pip install rhoknp
 ```
 
-## Documentation
-
-[https://rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/)
-
 ## Quick tour
 
-Let's start with using Juman++ with _rhoknp_.
-Here is a simple example of using Juman++ to analyze a sentence.
+Let's begin by using Juman++ with rhoknp.
+Here, we present a simple example demonstrating how Juman++ can be used to analyze a sentence.
 
 ```python
-# Perform language analysis by Juman++
+# Perform morphological analysis by Juman++
 jumanpp = rhoknp.Jumanpp()
 sentence = jumanpp.apply_to_sentence("電気抵抗率は電気の通しにくさを表す物性値である。")
 ```
 
-You can easily access the morphemes that make up the sentence.
+You can easily access the individual morphemes that make up the sentence.
 
 ```python
 for morpheme in sentence.morphemes:  # a.k.a. keitai-so
     ...
 ```
 
 Sentence objects can be saved in the JUMAN format.
@@ -121,33 +122,33 @@
     f.write(sentence.to_knp())
 
 # Load the sentence
 with open("sentence.knp", "rt") as f:
     sentence = rhoknp.Sentence.from_knp(f.read())
 ```
 
-_rhoknp_ also provides APIs for document-level language analysis.
+Furthermore, rhoknp provides convenient APIs for document-level language analysis.
 
 ```python
 document = rhoknp.Document.from_raw_text(
     "電気抵抗率は電気の通しにくさを表す物性値である。単に抵抗率とも呼ばれる。"
 )
 # If you know sentence boundaries, you can use `Document.from_sentences` instead.
 document = rhoknp.Document.from_sentences(
     [
         "電気抵抗率は電気の通しにくさを表す物性値である。",
         "単に抵抗率とも呼ばれる。",
     ]
 )
 ```
 
-Document objects can be handled in almost the same way as Sentence objects.
+Document objects can be handled in a similar manner as Sentence objects.
 
 ```python
-# Perform language analysis by Juman++
+# Perform morphological analysis by Juman++
 document = jumanpp.apply_to_document(document)
 
 # Access language units in the document
 for sentence in document.sentences:
     ...
 for morpheme in document.morphemes:
     ...
@@ -157,32 +158,32 @@
     f.write(document.to_jumanpp())
 
 # Load language analysis by Juman++
 with open("document.jumanpp", "rt") as f:
     document = rhoknp.Document.from_jumanpp(f.read())
 ```
 
-For more information, explore the [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/latest/).
+For more information, please refer to the [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/latest/).
 
 ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
 
-[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official Python binding for Juman++ and KNP.
-In _rhoknp_, we redesigned the API from the top-down, taking into account the current use cases of _pyknp_.
-The main differences are as follows:
-
-- **Support for document-level language analysis**: _rhoknp_ can load and instantiate the result of document-level language analysis (i.e., cohesion analysis and discourse relation analysis).
-- **Strictly type-aware**: _rhoknp_ is thoroughly annotated with type annotations.
-- **Extensive test suite**: _rhoknp_ is tested with an extensive test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
+[_pyknp_](https://pypi.org/project/pyknp/) serves as the official Python binding for Juman++ and KNP.
+In the development of rhoknp, we redesigned the API, considering the current use cases of pyknp.
+The key differences between the two are as follows:
+
+- **Support for document-level language analysis**: rhoknp allows you to load and instantiate the results of document-level language analysis, including cohesion analysis and discourse relation analysis.
+- **Strict type-awareness**: rhoknp has been thoroughly annotated with type annotations, ensuring strict type checking and improved code clarity.
+- **Comprehensive test suite**: rhoknp is extensively tested with a comprehensive test suite. You can view the code coverage report on [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
 
 ## License
 
 MIT
 
 ## Contributing
 
-We welcome contributions to _rhoknp_.
+We warmly welcome contributions to rhoknp.
 You can get started by reading the [contribution guide](https://rhoknp.readthedocs.io/en/latest/contributing/index.html).
 
 ## Reference
 
 - [KNP FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html)
 - [KNP - KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

#### html2text {}

```diff
@@ -1,72 +1,75 @@
                                  [rhoknp_logo]
      ****** rhoknp: Yet another Python binding for Juman++/KNP/KWJA ******
  [Test] [Codecov] [CodeFactor] [PyPI] [PyPI_-_Python_Version]_[Documentation]_
                              [Code_style_-_black]
-_rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp),
-[KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/
-kwja).[^1] [^1]: The logo was originally generated using OpenAI DALLÂ·E 2
-```python import rhoknp # Perform language analysis by Juman++ jumanpp =
-rhoknp.Jumanpp() sentence = jumanpp.apply_to_sentence
-( "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã" )
-# Access to the result for morpheme in sentence.morphemes: # a.k.a. keitai-so
-... # Save language analysis by Juman++ with open("result.jumanpp", "wt") as f:
-f.write(sentence.to_jumanpp()) # Load language analysis by Juman++ with open
-("result.jumanpp", "rt") as f: sentence = rhoknp.Sentence.from_jumanpp(f.read
-()) ``` ## Requirements - Python 3.7+ ## Optional requirements for language
-analysis - [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+ - [KNP]
-(https://github.com/ku-nlp/knp) 5.0+ - [KWJA](https://github.com/ku-nlp/kwja)
-1.0.0+ ## Installation ```shell pip install rhoknp ``` ## Documentation [https:
-//rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/
-) ## Quick tour Let's start with using Juman++ with _rhoknp_. Here is a simple
-example of using Juman++ to analyze a sentence. ```python # Perform language
+--- **Documentation**: [https://rhoknp.readthedocs.io/en/latest/](https://
+rhoknp.readthedocs.io/en/latest/) **Source Code**: [https://github.com/ku-nlp/
+rhoknp](https://github.com/ku-nlp/rhoknp) --- _rhoknp_ is a Python binding for
+[Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/
+knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1] [^1]: The logo was
+generated by OpenAI DALLÂ·E 2. ```python import rhoknp # Perform morphological
 analysis by Juman++ jumanpp = rhoknp.Jumanpp() sentence =
 jumanpp.apply_to_sentence
+( "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã" )
+# Access to the result for morpheme in sentence.morphemes: # a.k.a. keitai-so
+... # Save the result with open("result.jumanpp", "wt") as f: f.write
+(sentence.to_jumanpp()) # Load the result with open("result.jumanpp", "rt") as
+f: sentence = rhoknp.Sentence.from_jumanpp(f.read()) ``` ## Requirements -
+Python 3.7+ - (Optional) [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-
+rc3+ - (Optional) [KNP](https://github.com/ku-nlp/knp) 5.0+ - (Optional) [KWJA]
+(https://github.com/ku-nlp/kwja) 1.0.0+ ## Installation ```shell pip install
+rhoknp ``` ## Quick tour Let's begin by using Juman++ with rhoknp. Here, we
+present a simple example demonstrating how Juman++ can be used to analyze a
+sentence. ```python # Perform morphological analysis by Juman++ jumanpp =
+rhoknp.Jumanpp() sentence = jumanpp.apply_to_sentence
 ("é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã")
-``` You can easily access the morphemes that make up the sentence. ```python
-for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
-can be saved in the JUMAN format. ```python # Save the sentence in the JUMAN
-format with open("sentence.jumanpp", "wt") as f: f.write(sentence.to_jumanpp())
-# Load the sentence with open("sentence.jumanpp", "rt") as f: sentence =
-rhoknp.Sentence.from_jumanpp(f.read()) ``` Almost the same APIs are available
-for KNP. ```python # Perform language analysis by KNP knp = rhoknp.KNP()
-sentence = knp.apply_to_sentence
+``` You can easily access the individual morphemes that make up the sentence.
+```python for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ```
+Sentence objects can be saved in the JUMAN format. ```python # Save the
+sentence in the JUMAN format with open("sentence.jumanpp", "wt") as f: f.write
+(sentence.to_jumanpp()) # Load the sentence with open("sentence.jumanpp", "rt")
+as f: sentence = rhoknp.Sentence.from_jumanpp(f.read()) ``` Almost the same
+APIs are available for KNP. ```python # Perform language analysis by KNP knp =
+rhoknp.KNP() sentence = knp.apply_to_sentence
 ("é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã")
 ``` KNP performs language analysis at multiple levels. ```python for clause in
 sentence.clauses: # a.k.a., setsu ... for phrase in sentence.phrases: # a.k.a.
 bunsetsu ... for base_phrase in sentence.base_phrases: # a.k.a. kihon-ku ...
 for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
 can be saved in the KNP format. ```python # Save the sentence in the KNP format
 with open("sentence.knp", "wt") as f: f.write(sentence.to_knp()) # Load the
 sentence with open("sentence.knp", "rt") as f: sentence =
-rhoknp.Sentence.from_knp(f.read()) ``` _rhoknp_ also provides APIs for
-document-level language analysis. ```python document =
+rhoknp.Sentence.from_knp(f.read()) ``` Furthermore, rhoknp provides convenient
+APIs for document-level language analysis. ```python document =
 rhoknp.Document.from_raw_text
 (
 "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ãããåã«æµæçã¨ãå¼ã°ããã"
 ) # If you know sentence boundaries, you can use `Document.from_sentences`
 instead. document = rhoknp.Document.from_sentences(
 [ "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã",
 "åã«æµæçã¨ãå¼ã°ããã", ] ) ``` Document objects can be handled
-in almost the same way as Sentence objects. ```python # Perform language
+in a similar manner as Sentence objects. ```python # Perform morphological
 analysis by Juman++ document = jumanpp.apply_to_document(document) # Access
 language units in the document for sentence in document.sentences: ... for
 morpheme in document.morphemes: ... # Save language analysis by Juman++ with
 open("document.jumanpp", "wt") as f: f.write(document.to_jumanpp()) # Load
 language analysis by Juman++ with open("document.jumanpp", "rt") as f: document
-= rhoknp.Document.from_jumanpp(f.read()) ``` For more information, explore the
-[examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/
-latest/). ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
-[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official
-Python binding for Juman++ and KNP. In _rhoknp_, we redesigned the API from the
-top-down, taking into account the current use cases of _pyknp_. The main
-differences are as follows: - **Support for document-level language analysis**:
-_rhoknp_ can load and instantiate the result of document-level language
-analysis (i.e., cohesion analysis and discourse relation analysis). -
-**Strictly type-aware**: _rhoknp_ is thoroughly annotated with type
-annotations. - **Extensive test suite**: _rhoknp_ is tested with an extensive
-test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-
-nlp/rhoknp). ## License MIT ## Contributing We welcome contributions to
-_rhoknp_. You can get started by reading the [contribution guide](https://
-rhoknp.readthedocs.io/en/latest/contributing/index.html). ## Reference - [KNP
-FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html) - [KNP -
-KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
+= rhoknp.Document.from_jumanpp(f.read()) ``` For more information, please refer
+to the [examples](./examples) and [documentation](https://
+rhoknp.readthedocs.io/en/latest/). ## Main differences from [pyknp](https://
+github.com/ku-nlp/pyknp/) [_pyknp_](https://pypi.org/project/pyknp/) serves as
+the official Python binding for Juman++ and KNP. In the development of rhoknp,
+we redesigned the API, considering the current use cases of pyknp. The key
+differences between the two are as follows: - **Support for document-level
+language analysis**: rhoknp allows you to load and instantiate the results of
+document-level language analysis, including cohesion analysis and discourse
+relation analysis. - **Strict type-awareness**: rhoknp has been thoroughly
+annotated with type annotations, ensuring strict type checking and improved
+code clarity. - **Comprehensive test suite**: rhoknp is extensively tested with
+a comprehensive test suite. You can view the code coverage report on [Codecov]
+(https://app.codecov.io/gh/ku-nlp/rhoknp). ## License MIT ## Contributing We
+warmly welcome contributions to rhoknp. You can get started by reading the
+[contribution guide](https://rhoknp.readthedocs.io/en/latest/contributing/
+index.html). ## Reference - [KNP FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/
+~sasano/knp/format.html) - [KNP - KUROHASHI-CHU-MURAWAKI LAB](https://
+nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

### Comparing `rhoknp-1.3.1/pyproject.toml` & `rhoknp-1.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rhoknp"
-version = "1.3.1"
+version = "1.3.2"
 description = "Yet another Python binding for Juman++/KNP/KWJA"
 license = "MIT"
 authors = [
     "Hirokazu Kiyomaru <h.kiyomaru@gmail.com>",
     "Nobuhiro Ueda <ueda@nlp.ist.i.kyoto-u.ac.jp>",
 ]
 readme = "README.md"
```

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/cli.py` & `rhoknp-1.3.2/src/rhoknp/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,22 +75,24 @@
 
 
 @app.command(help="Serve an analyzer as HTTP server.")
 def serve(
     analyzer: AnalyzerType = typer.Argument(..., help="Analyzer to use. Choose from jumanpp, knp, kwja."),
     host: str = typer.Option("localhost", "--host", "-h", help="Host to listen on."),
     port: int = typer.Option(8000, "--port", "-p", help="Port to listen on."),
+    base_url: str = typer.Option("/", "--base-url", help="Root path of the server."),
     analyzer_args: Optional[List[str]] = typer.Argument(None, help="Additional arguments for the analyzer."),
 ) -> None:
     """解析器を起動し，HTTP サーバとして提供．
 
     Args:
         analyzer: 解析器の種類．
         host: ホスト．
         port: ポート．
+        base_url: ベース URL．
         analyzer_args: 解析器のオプション．
     """
-    serve_analyzer(analyzer, host, port, analyzer_args)  # pragma: no cover
+    serve_analyzer(analyzer, host, port, base_url, analyzer_args)  # pragma: no cover
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/serve.py` & `rhoknp-1.3.2/src/rhoknp/cli/serve.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,30 +106,23 @@
         spans.append(_Span(document.text[start:end], label))
         offset = end
     if offset < len(document.text):
         spans.append(_Span(document.text[offset:]))
     return spans
 
 
-def create_app(analyzer: AnalyzerType, *args, **kwargs) -> "fastapi.FastAPI":
+def create_app(analyzer: AnalyzerType, base_url: str = "/", *args, **kwargs) -> "fastapi.FastAPI":
     """解析器を起動し，HTTP サーバとして提供．
 
     Args:
         analyzer: 解析器の種類．
+        base_url: ベース URL．
         args: 解析器のオプション．
         kwargs: 解析器のオプション．
     """
-    app = fastapi.FastAPI()
-    app.mount("/static", fastapi.staticfiles.StaticFiles(directory=here.joinpath("static")), name="static")
-
-    templates = fastapi.templating.Jinja2Templates(directory=here.joinpath("templates"))
-    templates.env.globals["get_string_diff"] = _get_string_diff
-    templates.env.globals["draw_tree"] = _draw_tree
-    templates.env.globals["get_entity_spans"] = _get_entity_spans
-
     processor: Union[Jumanpp, KNP, KWJA]
     title: str
     template_name: str
     version: str
     if analyzer == AnalyzerType.JUMANPP:
         title = "Juman++ Demo"
         template_name = "jumanpp.jinja2"
@@ -142,44 +135,44 @@
         title = "KWJA Demo"
         template_name = "kwja.jinja2"
         processor = KWJA(*args, **kwargs)
     else:
         raise AssertionError  # unreachable
     version = processor.get_version()
 
+    app = fastapi.FastAPI()
+    app.mount("/static", fastapi.staticfiles.StaticFiles(directory=here.joinpath("static")), name="static")
+
+    templates = fastapi.templating.Jinja2Templates(directory=here.joinpath("templates"))
+    templates.env.globals["get_string_diff"] = _get_string_diff
+    templates.env.globals["draw_tree"] = _draw_tree
+    templates.env.globals["get_entity_spans"] = _get_entity_spans
+    templates.env.globals["title"] = title
+    templates.env.globals["version"] = version
+    templates.env.globals["base_url"] = base_url
+
     @app.exception_handler(_HTTPExceptionForIndex)
     async def http_exception_handler_for_index(request: fastapi.Request, exc: _HTTPExceptionForIndex):
         return templates.TemplateResponse(
             template_name,
-            {
-                "request": request,
-                "title": title,
-                "version": version,
-                "error": exc.detail,
-            },
+            {"request": request, "error": exc.detail},
             status_code=exc.status_code,
         )
 
     @app.get("/", response_class=fastapi.responses.HTMLResponse)
     async def index(request: fastapi.Request, text: str = ""):
         analyzed_document: Optional[Document] = None
         if text != "":
             try:
                 analyzed_document = processor.apply(text)
             except Exception as e:
                 raise _HTTPExceptionForIndex(fastapi.status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e))
         return templates.TemplateResponse(
             template_name,
-            {
-                "request": request,
-                "title": title,
-                "version": version,
-                "text": text,
-                "analyzed_document": analyzed_document,
-            },
+            {"request": request, "text": text, "analyzed_document": analyzed_document},
         )
 
     @app.exception_handler(_HTTPExceptionForAnalyze)
     async def http_exception_handler_for_analyze(request: fastapi.Request, exc: _HTTPExceptionForAnalyze):
         return fastapi.responses.JSONResponse(
             content={"error": {"code": exc.status_code, "message": exc.detail}},
             status_code=exc.status_code,
@@ -199,21 +192,22 @@
         except Exception as e:
             raise _HTTPExceptionForAnalyze(fastapi.status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e))
 
     return app
 
 
 def serve_analyzer(
-    analyzer: AnalyzerType, host: str, port: int, analyzer_args: Optional[List[str]]
+    analyzer: AnalyzerType, host: str, port: int, base_url: str, analyzer_args: Optional[List[str]]
 ) -> None:  # pragma: no cover
     """解析器を起動し，HTTP サーバとして提供．
 
     Args:
         analyzer: 解析器の種類．
         host: ホスト．
         port: ポート．
+        base_url: ベース URL．
         analyzer_args: 解析器のオプション．
     """
-    app = create_app(analyzer, options=analyzer_args)
+    app = create_app(analyzer, base_url, options=analyzer_args)
     config = uvicorn.Config(app, host=host, port=port)
     server = uvicorn.Server(config)
     server.run()
```

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/show.py` & `rhoknp-1.3.2/src/rhoknp/cli/show.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/static/css/style.css` & `rhoknp-1.3.2/src/rhoknp/cli/static/css/style.css`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 .result {
   margin: 0em 0.5em 1em;
   padding: 0.5em;
 }
 
 /* templates/components/named_entity_recognition.jinja2 */
 .entity {
-  padding: 0.45em 0.6em;
   margin: 0 0.25em;
   line-height: 1;
   border-radius: 0.35em;
 }
 
 .entity-organization {
   background: #7aecec;
```

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/static/images/apple-touch-icon.png` & `rhoknp-1.3.2/src/rhoknp/cli/static/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/static/images/favicon.ico` & `rhoknp-1.3.2/src/rhoknp/cli/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/static/js/script.js` & `rhoknp-1.3.2/src/rhoknp/cli/static/js/script.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /* Keep the status of the accordion to show analysis results */
 const defaultOpenAccordionItems = document.querySelectorAll(
-    ".accordion-item-default-open"
+    ".accordion-item-default-open",
 );
 defaultOpenAccordionItems.forEach((item) => {
     const itemId = `accordion-${item.id}`;
     if (localStorage.getItem(itemId) === null) {
         localStorage.setItem(itemId, "true");
     }
 });
```

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/stats.py` & `rhoknp-1.3.2/src/rhoknp/cli/stats.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/base.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/base.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <!DOCTYPE html>
 <html lang="ja">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <title>{{ title }}</title>
+    <base href="{{ base_url }}">
     <meta name="description" content="A web interface for Japanese text analyzer Juman++, KNP, and KWJA provided by rhoknp">
     <link
         rel="stylesheet"
         href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css"
         integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ"
         crossorigin="anonymous"
     >
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 
 
 
 
 
+
 {% include "components/navbar.jinja2" %}
 {% include "components/form.jinja2" %} {% if analyzed_document %}
 ===============================================================================
 {% include "components/raw_input.jinja2" %}
 * è§£æçµæ *
 {% include "components/show_all_button.jinja2" %} {% include "components/
 hide_all_button.jinja2" %} {% block result %} {% endblock %}
```

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/components/dependency_parsing.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/components/dependency_parsing.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/components/discourse_parsing.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/components/discourse_parsing.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/components/morphological_analysis.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/components/morphological_analysis.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/components/raw_output.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/components/raw_output.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/components/typo_correction.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/components/typo_correction.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/components/word_splitting.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/components/word_splitting.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/knp.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/knp.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cli/templates/kwja.jinja2` & `rhoknp-1.3.2/src/rhoknp/cli/templates/kwja.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/__init__.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/argument.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/argument.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/coreference.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/coreference.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/discourse.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/discourse.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/exophora.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/exophora.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/pas.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/pas.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/predicate.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/predicate.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/cohesion/rel.py` & `rhoknp-1.3.2/src/rhoknp/cohesion/rel.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/processors/jumanpp.py` & `rhoknp-1.3.2/src/rhoknp/processors/jumanpp.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/processors/knp.py` & `rhoknp-1.3.2/src/rhoknp/processors/knp.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/processors/kwja.py` & `rhoknp-1.3.2/src/rhoknp/processors/kwja.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/processors/processor.py` & `rhoknp-1.3.2/src/rhoknp/processors/processor.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/processors/senter.py` & `rhoknp-1.3.2/src/rhoknp/processors/senter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import re
-from typing import List, Union
+from typing import ClassVar, List, Union
 
 from rhoknp.processors.processor import Processor
 from rhoknp.units import Document, Sentence
 
 logger = logging.getLogger(__name__)
 
 
@@ -13,28 +13,28 @@
 
     Example:
         >>> from rhoknp import RegexSenter
         >>> senter = RegexSenter()
         >>> document = senter.apply("天気が良かったので散歩した。途中で先生に会った。")
     """
 
-    _PERIOD_PAT = re.compile(r"[。．？！♪☆★…?!]+")  #: ピリオドとみなすパターン．
+    _PERIOD_PAT: ClassVar[re.Pattern] = re.compile(r"[。．？！♪☆★…?!]+")  #: ピリオドとみなすパターン．
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}()"
 
     def apply_to_document(self, document: Union[Document, str]) -> Document:
         """文書に RegexSenter を適用する．
 
         Args:
             document: 文書．
         """
         if isinstance(document, str):
             document = Document(document)
-        sentence_texts = self._split_document(document.text)
+        sentence_texts: List[str] = self._split_document(document.text)
         return Document.from_sentences(sentence_texts)
 
     def apply_to_sentence(self, sentence: Union[Sentence, str]) -> Sentence:
         """文に RegexSenter を適用する．
 
         Args:
             sentence: 文．
@@ -43,25 +43,29 @@
             sentence = Sentence(sentence)
         return sentence
 
     def _split_document(self, text: str) -> List[str]:
         if text == "":
             return []
 
-        sentences: List[str] = []
-        for line in text.split("\n"):
-            # Split by periods
-            sentence_candidates: List[str] = []
+        def split_text_by_period(text: str) -> List[str]:
+            segments: List[str] = []
             start: int = 0
-            for match in self._PERIOD_PAT.finditer(line):
+            for match in self._PERIOD_PAT.finditer(text):
                 end: int = match.end()
-                sentence_candidates.append(line[start:end])
+                segments.append(text[start:end])
                 start = end
-            if start < len(line):
-                sentence_candidates.append(line[start:])
+            if start < len(text):
+                segments.append(text[start:])
+            return [segment.strip() for segment in segments]
+
+        sentences: List[str] = []
+        for line in text.split("\n"):
+            # Split by periods
+            sentence_candidates: List[str] = split_text_by_period(line)
 
             # Merge sentence candidates so that strings in parentheses or brackets are not split
             parenthesis_level: int = 0
             hook_bracket_level: int = 0
             double_hook_bracket_level: int = 0
             sentence: str = ""
             while sentence_candidates:
@@ -74,10 +78,10 @@
                 hook_bracket_level += sentence_candidate.count("「") - sentence_candidate.count("」")
                 double_hook_bracket_level += sentence_candidate.count("『") - sentence_candidate.count("』")
                 if parenthesis_level == hook_bracket_level == double_hook_bracket_level == 0:
                     if sentence.strip():
                         sentences.append(sentence.strip())
                     sentence = ""
             if sentence.strip():
-                sentences.append(sentence.strip())
+                sentences.extend(split_text_by_period(sentence.strip()))
 
         return sentences
```

### Comparing `rhoknp-1.3.1/src/rhoknp/props/feature.py` & `rhoknp-1.3.2/src/rhoknp/props/feature.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/props/memo.py` & `rhoknp-1.3.2/src/rhoknp/props/memo.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/props/named_entity.py` & `rhoknp-1.3.2/src/rhoknp/props/named_entity.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/props/semantics.py` & `rhoknp-1.3.2/src/rhoknp/props/semantics.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/units/base_phrase.py` & `rhoknp-1.3.2/src/rhoknp/units/base_phrase.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/units/clause.py` & `rhoknp-1.3.2/src/rhoknp/units/clause.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/units/document.py` & `rhoknp-1.3.2/src/rhoknp/units/document.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/units/morpheme.py` & `rhoknp-1.3.2/src/rhoknp/units/morpheme.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/units/phrase.py` & `rhoknp-1.3.2/src/rhoknp/units/phrase.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/units/sentence.py` & `rhoknp-1.3.2/src/rhoknp/units/sentence.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/units/unit.py` & `rhoknp-1.3.2/src/rhoknp/units/unit.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/utils/reader.py` & `rhoknp-1.3.2/src/rhoknp/utils/reader.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/src/rhoknp/utils/util.py` & `rhoknp-1.3.2/src/rhoknp/utils/util.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.1/PKG-INFO` & `rhoknp-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhoknp
-Version: 1.3.1
+Version: 1.3.2
 Summary: Yet another Python binding for Juman++/KNP/KWJA
 Home-page: https://github.com/ku-nlp/rhoknp
 License: MIT
 Keywords: NLP
 Author: Hirokazu Kiyomaru
 Author-email: h.kiyomaru@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -43,72 +43,73 @@
 <a href="https://www.codefactor.io/repository/github/ku-nlp/rhoknp"><img alt="CodeFactor" src="https://img.shields.io/codefactor/grade/github/ku-nlp/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rhoknp?style=flat-square">
 <a href="https://rhoknp.readthedocs.io/en/latest/"><img alt="Documentation" src="https://img.shields.io/readthedocs/rhoknp?style=flat-square"></a>
 <a href="https://github.com/psf/black"><img alt="Code style - black" src="https://img.shields.io/badge/code%20style-black-222222?style=flat-square"></a>
 </p>
 
+---
+
+**Documentation**: [https://rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/)
+
+**Source Code**: [https://github.com/ku-nlp/rhoknp](https://github.com/ku-nlp/rhoknp)
+
+---
+
 _rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1]
 
-[^1]: The logo was originally generated using OpenAI DALL·E 2
+[^1]: The logo was generated by OpenAI DALL·E 2.
 
 ```python
 import rhoknp
 
-# Perform language analysis by Juman++
+# Perform morphological analysis by Juman++
 jumanpp = rhoknp.Jumanpp()
 sentence = jumanpp.apply_to_sentence(
     "電気抵抗率は電気の通しにくさを表す物性値である。"
 )
 
 # Access to the result
 for morpheme in sentence.morphemes:  # a.k.a. keitai-so
     ...
 
-# Save language analysis by Juman++
+# Save the result
 with open("result.jumanpp", "wt") as f:
     f.write(sentence.to_jumanpp())
 
-# Load language analysis by Juman++
+# Load the result
 with open("result.jumanpp", "rt") as f:
     sentence = rhoknp.Sentence.from_jumanpp(f.read())
 ```
 
 ## Requirements
 
 - Python 3.7+
-
-## Optional requirements for language analysis
-
-- [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+
-- [KNP](https://github.com/ku-nlp/knp) 5.0+
-- [KWJA](https://github.com/ku-nlp/kwja) 1.0.0+
+- (Optional) [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+
+- (Optional) [KNP](https://github.com/ku-nlp/knp) 5.0+
+- (Optional) [KWJA](https://github.com/ku-nlp/kwja) 1.0.0+
 
 ## Installation
 
 ```shell
 pip install rhoknp
 ```
 
-## Documentation
-
-[https://rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/)
-
 ## Quick tour
 
-Let's start with using Juman++ with _rhoknp_.
-Here is a simple example of using Juman++ to analyze a sentence.
+Let's begin by using Juman++ with rhoknp.
+Here, we present a simple example demonstrating how Juman++ can be used to analyze a sentence.
 
 ```python
-# Perform language analysis by Juman++
+# Perform morphological analysis by Juman++
 jumanpp = rhoknp.Jumanpp()
 sentence = jumanpp.apply_to_sentence("電気抵抗率は電気の通しにくさを表す物性値である。")
 ```
 
-You can easily access the morphemes that make up the sentence.
+You can easily access the individual morphemes that make up the sentence.
 
 ```python
 for morpheme in sentence.morphemes:  # a.k.a. keitai-so
     ...
 ```
 
 Sentence objects can be saved in the JUMAN format.
@@ -152,33 +153,33 @@
     f.write(sentence.to_knp())
 
 # Load the sentence
 with open("sentence.knp", "rt") as f:
     sentence = rhoknp.Sentence.from_knp(f.read())
 ```
 
-_rhoknp_ also provides APIs for document-level language analysis.
+Furthermore, rhoknp provides convenient APIs for document-level language analysis.
 
 ```python
 document = rhoknp.Document.from_raw_text(
     "電気抵抗率は電気の通しにくさを表す物性値である。単に抵抗率とも呼ばれる。"
 )
 # If you know sentence boundaries, you can use `Document.from_sentences` instead.
 document = rhoknp.Document.from_sentences(
     [
         "電気抵抗率は電気の通しにくさを表す物性値である。",
         "単に抵抗率とも呼ばれる。",
     ]
 )
 ```
 
-Document objects can be handled in almost the same way as Sentence objects.
+Document objects can be handled in a similar manner as Sentence objects.
 
 ```python
-# Perform language analysis by Juman++
+# Perform morphological analysis by Juman++
 document = jumanpp.apply_to_document(document)
 
 # Access language units in the document
 for sentence in document.sentences:
     ...
 for morpheme in document.morphemes:
     ...
@@ -188,33 +189,33 @@
     f.write(document.to_jumanpp())
 
 # Load language analysis by Juman++
 with open("document.jumanpp", "rt") as f:
     document = rhoknp.Document.from_jumanpp(f.read())
 ```
 
-For more information, explore the [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/latest/).
+For more information, please refer to the [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/latest/).
 
 ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
 
-[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official Python binding for Juman++ and KNP.
-In _rhoknp_, we redesigned the API from the top-down, taking into account the current use cases of _pyknp_.
-The main differences are as follows:
-
-- **Support for document-level language analysis**: _rhoknp_ can load and instantiate the result of document-level language analysis (i.e., cohesion analysis and discourse relation analysis).
-- **Strictly type-aware**: _rhoknp_ is thoroughly annotated with type annotations.
-- **Extensive test suite**: _rhoknp_ is tested with an extensive test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
+[_pyknp_](https://pypi.org/project/pyknp/) serves as the official Python binding for Juman++ and KNP.
+In the development of rhoknp, we redesigned the API, considering the current use cases of pyknp.
+The key differences between the two are as follows:
+
+- **Support for document-level language analysis**: rhoknp allows you to load and instantiate the results of document-level language analysis, including cohesion analysis and discourse relation analysis.
+- **Strict type-awareness**: rhoknp has been thoroughly annotated with type annotations, ensuring strict type checking and improved code clarity.
+- **Comprehensive test suite**: rhoknp is extensively tested with a comprehensive test suite. You can view the code coverage report on [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
 
 ## License
 
 MIT
 
 ## Contributing
 
-We welcome contributions to _rhoknp_.
+We warmly welcome contributions to rhoknp.
 You can get started by reading the [contribution guide](https://rhoknp.readthedocs.io/en/latest/contributing/index.html).
 
 ## Reference
 
 - [KNP FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html)
 - [KNP - KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rhoknp Version: 1.3.1 Summary: Yet another Python
+Metadata-Version: 2.1 Name: rhoknp Version: 1.3.2 Summary: Yet another Python
 binding for Juman++/KNP/KWJA Home-page: https://github.com/ku-nlp/rhoknp
 License: MIT Keywords: NLP Author: Hirokazu Kiyomaru Author-email:
 h.kiyomaru@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -16,75 +16,78 @@
 == "cli") Requires-Dist: uvicorn (>=0.21.0,<1) ; extra == "cli" Project-URL:
 Documentation, https://rhoknp.readthedocs.io/en/latest Project-URL: Repository,
 https://github.com/ku-nlp/rhoknp Description-Content-Type: text/markdown
                                  [rhoknp_logo]
      ****** rhoknp: Yet another Python binding for Juman++/KNP/KWJA ******
  [Test] [Codecov] [CodeFactor] [PyPI] [PyPI_-_Python_Version]_[Documentation]_
                              [Code_style_-_black]
-_rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp),
-[KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/
-kwja).[^1] [^1]: The logo was originally generated using OpenAI DALLÂ·E 2
-```python import rhoknp # Perform language analysis by Juman++ jumanpp =
-rhoknp.Jumanpp() sentence = jumanpp.apply_to_sentence
-( "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã" )
-# Access to the result for morpheme in sentence.morphemes: # a.k.a. keitai-so
-... # Save language analysis by Juman++ with open("result.jumanpp", "wt") as f:
-f.write(sentence.to_jumanpp()) # Load language analysis by Juman++ with open
-("result.jumanpp", "rt") as f: sentence = rhoknp.Sentence.from_jumanpp(f.read
-()) ``` ## Requirements - Python 3.7+ ## Optional requirements for language
-analysis - [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+ - [KNP]
-(https://github.com/ku-nlp/knp) 5.0+ - [KWJA](https://github.com/ku-nlp/kwja)
-1.0.0+ ## Installation ```shell pip install rhoknp ``` ## Documentation [https:
-//rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/
-) ## Quick tour Let's start with using Juman++ with _rhoknp_. Here is a simple
-example of using Juman++ to analyze a sentence. ```python # Perform language
+--- **Documentation**: [https://rhoknp.readthedocs.io/en/latest/](https://
+rhoknp.readthedocs.io/en/latest/) **Source Code**: [https://github.com/ku-nlp/
+rhoknp](https://github.com/ku-nlp/rhoknp) --- _rhoknp_ is a Python binding for
+[Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/
+knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1] [^1]: The logo was
+generated by OpenAI DALLÂ·E 2. ```python import rhoknp # Perform morphological
 analysis by Juman++ jumanpp = rhoknp.Jumanpp() sentence =
 jumanpp.apply_to_sentence
+( "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã" )
+# Access to the result for morpheme in sentence.morphemes: # a.k.a. keitai-so
+... # Save the result with open("result.jumanpp", "wt") as f: f.write
+(sentence.to_jumanpp()) # Load the result with open("result.jumanpp", "rt") as
+f: sentence = rhoknp.Sentence.from_jumanpp(f.read()) ``` ## Requirements -
+Python 3.7+ - (Optional) [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-
+rc3+ - (Optional) [KNP](https://github.com/ku-nlp/knp) 5.0+ - (Optional) [KWJA]
+(https://github.com/ku-nlp/kwja) 1.0.0+ ## Installation ```shell pip install
+rhoknp ``` ## Quick tour Let's begin by using Juman++ with rhoknp. Here, we
+present a simple example demonstrating how Juman++ can be used to analyze a
+sentence. ```python # Perform morphological analysis by Juman++ jumanpp =
+rhoknp.Jumanpp() sentence = jumanpp.apply_to_sentence
 ("é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã")
-``` You can easily access the morphemes that make up the sentence. ```python
-for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
-can be saved in the JUMAN format. ```python # Save the sentence in the JUMAN
-format with open("sentence.jumanpp", "wt") as f: f.write(sentence.to_jumanpp())
-# Load the sentence with open("sentence.jumanpp", "rt") as f: sentence =
-rhoknp.Sentence.from_jumanpp(f.read()) ``` Almost the same APIs are available
-for KNP. ```python # Perform language analysis by KNP knp = rhoknp.KNP()
-sentence = knp.apply_to_sentence
+``` You can easily access the individual morphemes that make up the sentence.
+```python for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ```
+Sentence objects can be saved in the JUMAN format. ```python # Save the
+sentence in the JUMAN format with open("sentence.jumanpp", "wt") as f: f.write
+(sentence.to_jumanpp()) # Load the sentence with open("sentence.jumanpp", "rt")
+as f: sentence = rhoknp.Sentence.from_jumanpp(f.read()) ``` Almost the same
+APIs are available for KNP. ```python # Perform language analysis by KNP knp =
+rhoknp.KNP() sentence = knp.apply_to_sentence
 ("é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã")
 ``` KNP performs language analysis at multiple levels. ```python for clause in
 sentence.clauses: # a.k.a., setsu ... for phrase in sentence.phrases: # a.k.a.
 bunsetsu ... for base_phrase in sentence.base_phrases: # a.k.a. kihon-ku ...
 for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
 can be saved in the KNP format. ```python # Save the sentence in the KNP format
 with open("sentence.knp", "wt") as f: f.write(sentence.to_knp()) # Load the
 sentence with open("sentence.knp", "rt") as f: sentence =
-rhoknp.Sentence.from_knp(f.read()) ``` _rhoknp_ also provides APIs for
-document-level language analysis. ```python document =
+rhoknp.Sentence.from_knp(f.read()) ``` Furthermore, rhoknp provides convenient
+APIs for document-level language analysis. ```python document =
 rhoknp.Document.from_raw_text
 (
 "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ãããåã«æµæçã¨ãå¼ã°ããã"
 ) # If you know sentence boundaries, you can use `Document.from_sentences`
 instead. document = rhoknp.Document.from_sentences(
 [ "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã",
 "åã«æµæçã¨ãå¼ã°ããã", ] ) ``` Document objects can be handled
-in almost the same way as Sentence objects. ```python # Perform language
+in a similar manner as Sentence objects. ```python # Perform morphological
 analysis by Juman++ document = jumanpp.apply_to_document(document) # Access
 language units in the document for sentence in document.sentences: ... for
 morpheme in document.morphemes: ... # Save language analysis by Juman++ with
 open("document.jumanpp", "wt") as f: f.write(document.to_jumanpp()) # Load
 language analysis by Juman++ with open("document.jumanpp", "rt") as f: document
-= rhoknp.Document.from_jumanpp(f.read()) ``` For more information, explore the
-[examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/
-latest/). ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
-[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official
-Python binding for Juman++ and KNP. In _rhoknp_, we redesigned the API from the
-top-down, taking into account the current use cases of _pyknp_. The main
-differences are as follows: - **Support for document-level language analysis**:
-_rhoknp_ can load and instantiate the result of document-level language
-analysis (i.e., cohesion analysis and discourse relation analysis). -
-**Strictly type-aware**: _rhoknp_ is thoroughly annotated with type
-annotations. - **Extensive test suite**: _rhoknp_ is tested with an extensive
-test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-
-nlp/rhoknp). ## License MIT ## Contributing We welcome contributions to
-_rhoknp_. You can get started by reading the [contribution guide](https://
-rhoknp.readthedocs.io/en/latest/contributing/index.html). ## Reference - [KNP
-FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html) - [KNP -
-KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
+= rhoknp.Document.from_jumanpp(f.read()) ``` For more information, please refer
+to the [examples](./examples) and [documentation](https://
+rhoknp.readthedocs.io/en/latest/). ## Main differences from [pyknp](https://
+github.com/ku-nlp/pyknp/) [_pyknp_](https://pypi.org/project/pyknp/) serves as
+the official Python binding for Juman++ and KNP. In the development of rhoknp,
+we redesigned the API, considering the current use cases of pyknp. The key
+differences between the two are as follows: - **Support for document-level
+language analysis**: rhoknp allows you to load and instantiate the results of
+document-level language analysis, including cohesion analysis and discourse
+relation analysis. - **Strict type-awareness**: rhoknp has been thoroughly
+annotated with type annotations, ensuring strict type checking and improved
+code clarity. - **Comprehensive test suite**: rhoknp is extensively tested with
+a comprehensive test suite. You can view the code coverage report on [Codecov]
+(https://app.codecov.io/gh/ku-nlp/rhoknp). ## License MIT ## Contributing We
+warmly welcome contributions to rhoknp. You can get started by reading the
+[contribution guide](https://rhoknp.readthedocs.io/en/latest/contributing/
+index.html). ## Reference - [KNP FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/
+~sasano/knp/format.html) - [KNP - KUROHASHI-CHU-MURAWAKI LAB](https://
+nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

