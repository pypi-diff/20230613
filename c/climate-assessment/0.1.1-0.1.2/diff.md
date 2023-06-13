# Comparing `tmp/climate-assessment-0.1.1.tar.gz` & `tmp/climate-assessment-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate-assessment-0.1.1.tar", last modified: Thu Jun 30 08:09:44 2022, max compression
+gzip compressed data, was "climate-assessment-0.1.2.tar", last modified: Tue Jun 13 15:42:38 2023, max compression
```

## Comparing `climate-assessment-0.1.1.tar` & `climate-assessment-0.1.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.614955 climate-assessment-0.1.1/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      226 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/.dockerignore
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      965 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/.env.sample
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2035 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/.gitignore
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      107 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/.readthedocs.yml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      983 2022-06-28 07:24:04.000000 climate-assessment-0.1.1/CHANGELOG.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1393 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/CITATION.cff
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      588 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/Dockerfile
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1073 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/LICENSE
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       44 2022-06-28 07:24:04.000000 climate-assessment-0.1.1/MANIFEST.in
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3650 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/Makefile
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4328 2022-06-30 08:09:44.614955 climate-assessment-0.1.1/PKG-INFO
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3034 2022-06-28 09:41:09.000000 climate-assessment-0.1.1/README.rst
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/data/
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/data/cicero/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   295394 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/data/cicero/subset_cscm_configfile.json
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     9175 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/data/emissions_variable_list_climateruns.xlsx
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/doc/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      634 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/doc/Makefile
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3337 2022-06-21 15:23:17.000000 climate-assessment-0.1.1/doc/NOTICE.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      867 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/doc/README.rst
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/doc/_static/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        0 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/doc/_static/.gitkeep
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   305539 2022-06-08 09:35:56.000000 climate-assessment-0.1.1/doc/_static/category_flowchart.jpg
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    86790 2022-06-08 09:35:56.000000 climate-assessment-0.1.1/doc/_static/overview_workflow.png
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2558 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/doc/code.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2500 2022-06-21 15:23:17.000000 climate-assessment-0.1.1/doc/conf.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1272 2022-06-08 09:35:56.000000 climate-assessment-0.1.1/doc/dev.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    10838 2022-06-08 09:35:56.000000 climate-assessment-0.1.1/doc/emulator.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    61792 2022-06-21 15:23:17.000000 climate-assessment-0.1.1/doc/general.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     5048 2022-06-21 15:23:17.000000 climate-assessment-0.1.1/doc/index.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3219 2022-06-28 07:24:04.000000 climate-assessment-0.1.1/doc/install.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      760 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/doc/make.bat
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1584 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/doc/prereqs.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1540 2022-06-08 09:35:56.000000 climate-assessment-0.1.1/doc/user_guide.rst
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      714 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/doc/utility.rst
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/notebooks/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        0 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/notebooks/.gitkeep
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     9853 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/notebooks/run-example-ciceroscm.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13107 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/notebooks/run-example-custom.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    11556 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/notebooks/run-example-fair.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13020 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/notebooks/run-example-magicc.ipynb
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      109 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/run_docker.sh
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/scripts/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2125 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/generate-magicc-sr15-input-files.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      161 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_clim.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      177 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_create_infillerdatabase.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      100 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_extract_ips.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      162 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_harm.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      173 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_harm_inf.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      159 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_infilling.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      164 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_postprocess.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      117 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_split_scenarios.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      161 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/scripts/run_workflow.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2281 2022-06-30 08:09:44.614955 climate-assessment-0.1.1/setup.cfg
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       58 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/setup.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.606955 climate-assessment-0.1.1/src/
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/src/climate_assessment/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      853 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    38775 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/src/climate_assessment/checks.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    33528 2022-06-21 15:23:17.000000 climate-assessment-0.1.1/src/climate_assessment/cli.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.614955 climate-assessment-0.1.1/src/climate_assessment/climate/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    16392 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/climate/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      830 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/climate/ciceroscm.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3505 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/climate/fair.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4713 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/climate/magicc7.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    17320 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/climate/post_process.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    12231 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/climate/variable_definitions.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2385 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/climate/wg3.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.614955 climate-assessment-0.1.1/src/climate_assessment/harmonization/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13035 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      174 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/aneris_ar6.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      173 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/aneris_ar6_co2.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      175 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/aneris_sr15.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      174 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/aneris_sr15_co2.yaml
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    68340 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/history_ar6.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    68367 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/history_sr15.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       69 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization/regions_ar6.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4469 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/harmonization_and_infilling.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.614955 climate-assessment-0.1.1/src/climate_assessment/infilling/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    19255 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/infilling/__init__.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   799351 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2627 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/postprocess.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1960 2022-06-23 12:44:15.000000 climate-assessment-0.1.1/src/climate_assessment/testing.py
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    16432 2022-06-08 09:09:41.000000 climate-assessment-0.1.1/src/climate_assessment/utils.py
-drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2022-06-30 08:09:44.610955 climate-assessment-0.1.1/src/climate_assessment.egg-info/
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4328 2022-06-30 08:09:43.000000 climate-assessment-0.1.1/src/climate_assessment.egg-info/PKG-INFO
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2325 2022-06-30 08:09:44.000000 climate-assessment-0.1.1/src/climate_assessment.egg-info/SOURCES.txt
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        1 2022-06-30 08:09:43.000000 climate-assessment-0.1.1/src/climate_assessment.egg-info/dependency_links.txt
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      641 2022-06-30 08:09:43.000000 climate-assessment-0.1.1/src/climate_assessment.egg-info/requires.txt
--rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       19 2022-06-30 08:09:43.000000 climate-assessment-0.1.1/src/climate_assessment.egg-info/top_level.txt
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      226 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/.dockerignore
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      965 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/.env.sample
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2035 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/.gitignore
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      107 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/.readthedocs.yml
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1074 2023-06-13 15:33:48.000000 climate-assessment-0.1.2/CHANGELOG.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1393 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/CITATION.cff
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      588 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/Dockerfile
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1073 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/LICENSE
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       44 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/MANIFEST.in
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3650 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/Makefile
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4289 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/PKG-INFO
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3034 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/README.rst
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.528253 climate-assessment-0.1.2/data/
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.528253 climate-assessment-0.1.2/data/cicero/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   295394 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/data/cicero/subset_cscm_configfile.json
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     9175 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/data/emissions_variable_list_climateruns.xlsx
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.536253 climate-assessment-0.1.2/doc/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      634 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/Makefile
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3583 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/NOTICE.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      867 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/README.rst
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.540253 climate-assessment-0.1.2/doc/_static/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        0 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/_static/.gitkeep
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   305539 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/_static/category_flowchart.jpg
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    86790 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/_static/overview_workflow.png
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2558 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/code.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2500 2022-06-21 15:23:17.000000 climate-assessment-0.1.2/doc/conf.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1272 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/dev.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    10916 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/emulator.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    61922 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/general.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     5071 2023-06-13 15:33:54.000000 climate-assessment-0.1.2/doc/index.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3219 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/doc/install.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      760 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/make.bat
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1584 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/prereqs.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1540 2022-06-08 09:35:56.000000 climate-assessment-0.1.2/doc/user_guide.rst
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      714 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/doc/utility.rst
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.540253 climate-assessment-0.1.2/notebooks/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        0 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/notebooks/.gitkeep
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     9853 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-ciceroscm.ipynb
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13107 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-custom.ipynb
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    11556 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-fair.ipynb
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13020 2023-05-11 09:56:20.000000 climate-assessment-0.1.2/notebooks/run-example-magicc.ipynb
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      109 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/run_docker.sh
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.544252 climate-assessment-0.1.2/scripts/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2125 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/generate-magicc-sr15-input-files.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      161 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_clim.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      177 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_create_infillerdatabase.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      100 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_extract_ips.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      162 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_harm.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      173 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_harm_inf.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      159 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_infilling.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      164 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_postprocess.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      117 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_split_scenarios.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      161 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/scripts/run_workflow.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2262 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/setup.cfg
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       58 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/setup.py
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.524253 climate-assessment-0.1.2/src/
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.548252 climate-assessment-0.1.2/src/climate_assessment/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      853 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/__init__.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    38775 2023-06-13 15:33:48.000000 climate-assessment-0.1.2/src/climate_assessment/checks.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    33528 2022-06-21 15:23:17.000000 climate-assessment-0.1.2/src/climate_assessment/cli.py
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.556252 climate-assessment-0.1.2/src/climate_assessment/climate/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    16426 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/climate/__init__.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      830 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/ciceroscm.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     3505 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/fair.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4713 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/magicc7.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    17320 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/post_process.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    12231 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/variable_definitions.csv
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2385 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/climate/wg3.py
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.556252 climate-assessment-0.1.2/src/climate_assessment/harmonization/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    13035 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/__init__.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      174 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_ar6.yaml
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      173 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_ar6_co2.yaml
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      175 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_sr15.yaml
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      174 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/aneris_sr15_co2.yaml
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    68340 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/history_ar6.csv
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    68367 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/history_sr15.csv
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       69 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization/regions_ar6.csv
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4469 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/harmonization_and_infilling.py
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.560252 climate-assessment-0.1.2/src/climate_assessment/infilling/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    19254 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/infilling/__init__.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)   799351 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2627 2022-06-08 09:09:41.000000 climate-assessment-0.1.2/src/climate_assessment/postprocess.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     1878 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/testing.py
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)    16431 2023-05-17 09:02:43.000000 climate-assessment-0.1.2/src/climate_assessment/utils.py
+drwxrwxr-x   0 hackstock  (1000) hackstock  (1000)        0 2023-06-13 15:42:38.552252 climate-assessment-0.1.2/src/climate_assessment.egg-info/
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     4289 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/PKG-INFO
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)     2325 2023-06-13 15:42:38.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/SOURCES.txt
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)        1 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/dependency_links.txt
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)      662 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/requires.txt
+-rw-rw-r--   0 hackstock  (1000) hackstock  (1000)       19 2023-06-13 15:42:37.000000 climate-assessment-0.1.2/src/climate_assessment.egg-info/top_level.txt
```

### Comparing `climate-assessment-0.1.1/.env.sample` & `climate-assessment-0.1.2/.env.sample`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/.gitignore` & `climate-assessment-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/CHANGELOG.rst` & `climate-assessment-0.1.2/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     - Security: in case of vulnerabilities.
 
 master
 ------
 
 Added
 ~~~~~
+- (`#31 https://github.com/iiasa/climate-assessment/pull/31`_) Update pyam-iamc to >=1.7.0
 - (`#15 <https://github.com/iiasa/climate-assessment/pull/15>`_) Fix packaging issues and add installation instructions
 - (`#6 <https://github.com/iiasa/climate-assessment/pull/6>`_) Added example run notebooks and tests thereof
 - (`#1 <https://github.com/iiasa/climate-assessment/pull/1>`_) Added :func:`climate_assessment.cli.run_workflow`
 
 
 v0.1.0 - 2022-06-08
 -------------------
```

### Comparing `climate-assessment-0.1.1/CITATION.cff` & `climate-assessment-0.1.2/CITATION.cff`

 * *Files 7% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     orcid: 'https://orcid.org/0000-0002-1482-1366'
 repository-code: 'https://github.com/iiasa/climate-assessment'
 license: MIT
 identifiers:
   - description: The concept DOI of the work.
     type: doi
     value: 10.5281/zenodo.6624519    
-  - description: The versioned DOI for version 0.1.0 of the work.
+  - description: The versioned DOI for version 0.1.1 of the work.
     type: doi
-    value: 10.5281/zenodo.6624520
+    value: 10.5281/zenodo.6782457
```

### Comparing `climate-assessment-0.1.1/Dockerfile` & `climate-assessment-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/LICENSE` & `climate-assessment-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/Makefile` & `climate-assessment-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/PKG-INFO` & `climate-assessment-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: climate-assessment
-Version: 0.1.1
+Version: 0.1.2
 Summary: Climate assessment of long-term emissions pathways: IPCC AR6 WGIII version
 Home-page: https://github.com/iiasa/climate-assessment
 Author: Jarmo S. Kikstra, Zebedee R.J. Nicholls, Jared Lewis, Christopher J. Smith, Robin D. Lamboll, Edward Byers, Marit Sandstad, Laura Wienpahl, Philip Hackstock
 Author-email: kikstra@iiasa.ac.at
 License: MIT License
 Project-URL: Source, http://github.com/iiasa/climate-assessment
-Project-URL: Documentation, https://iiasa-energy-program-climate-assessment.readthedocs-hosted.com/en/latest/
+Project-URL: Documentation, https://climate-assessment.readthedocs.io/
 Project-URL: Bug_Reports, https://github.com/iiasa/climate-assessment/issues
 Keywords: climate,integrated assessment,emissions,temperature,IPCC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `climate-assessment-0.1.1/README.rst` & `climate-assessment-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/data/cicero/subset_cscm_configfile.json` & `climate-assessment-0.1.2/data/cicero/subset_cscm_configfile.json`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/data/emissions_variable_list_climateruns.xlsx` & `climate-assessment-0.1.2/data/emissions_variable_list_climateruns.xlsx`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/Makefile` & `climate-assessment-0.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/NOTICE.rst` & `climate-assessment-0.1.2/doc/NOTICE.rst`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,30 @@
     Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
 
 .. _notice-cite:
 
 2. Cite the scientific publication
 ==================================
 
-Cite, at minimum, the following manuscript (exact citation TBD.):
+Cite, at minimum, the following manuscript:
 
   | Jarmo S. Kikstra, Zebedee R. J. Nicholls, Christopher J. Smith, Jared Lewis, Robin D. Lamboll, Edward Byers, Marit Sandstad, Malte Meinshausen, Matthew J. Gidden, Joeri Rogelj, Elmar Kriegler, Glen P. Peters, Jan S. Fuglestvedt, Ragnhild B. Skeie, Bjørn H. Samset, Laura Wienpahl, Detlef P. van Vuuren, Kaj-Ivar van der Wijst, Alaa Al Khourdajie, Piers M. Forster, Andy Reisinger, Roberto Schaeffer, and Keywan Riahi
   | "The IPCC Sixth Assessment Report WGIII climate assessment of mitigation pathways: from emissions to global temperatures".
-  | *Geosci. Model Dev.*
-  | (in review)
+  | *Geosci. Model Dev., 15, 9075–9109*
+  | https://doi.org/10.5194/gmd-15-9075-2022
+  | 2022
 
 Additionally, you may cite the source code using the Zenodo reference (DOI: https://doi.org/10.5281/zenodo.6624519).
 
-If you are using the AR6 scenario data (DOI: https://doi.org/10.5281/zenodo.6390767) and the AR6 infiller database (DOI: https://doi.org/10.5281/zenodo.6390767), you should in addition cite those respective sources.
+If you are using the AR6 scenario data (DOI: https://doi.org/10.5281/zenodo.5886911) and the AR6 infiller database (DOI: https://doi.org/10.5281/zenodo.6390767), you should in addition cite those respective sources.
 
 In addition, to provide credit to the climate emulator modelers, please cite literature describing the climate emulator(s) that you use.
 
 Lastly, you may cite the tools that enabled the development of this climate assessment workflow, including ``aneris``, ``silicone``, and ``openscm-runner``.
 
 All these citations are also provided in full in the manuscript mentioned above, if further guidance is required on how to cite specific tools and data.
 
 - **Cite the code via Zenodo**.
-  The `DOI 10.5281/zenodo.6624520 <https://doi.org/10.5281/zenodo.6624519>`_ represents *all* versions of the :mod:`climate-assessment` code, and will always resolve to the latest version.
+  The `DOI 10.5281/zenodo.6624519 <https://doi.org/10.5281/zenodo.6624519>`_ represents *all* versions of the :mod:`climate-assessment` code, and will always resolve to the latest version.
   Zenodo also provides citation export in BibTeX and other formats.
+  If you would like to cite a specific release version, that is possible too and requires using the dedicate URLs, such as `DOI 10.5281/zenodo.6782457 <https://doi.org/10.5281/zenodo.6782457>` for version v0.1.1.
 - Include a link, e.g. in a footnote, to the online documentation at https://climate-assessment.readthedocs.io.
```

### Comparing `climate-assessment-0.1.1/doc/README.rst` & `climate-assessment-0.1.2/doc/README.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/_static/category_flowchart.jpg` & `climate-assessment-0.1.2/doc/_static/category_flowchart.jpg`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/_static/overview_workflow.png` & `climate-assessment-0.1.2/doc/_static/overview_workflow.png`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/code.rst` & `climate-assessment-0.1.2/doc/code.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/conf.py` & `climate-assessment-0.1.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/dev.rst` & `climate-assessment-0.1.2/doc/dev.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/emulator.rst` & `climate-assessment-0.1.2/doc/emulator.rst`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,21 @@
 
 Emulator-specific functions
 ---------------------------
 .. autofunction:: climate_assessment.climate.get_magicc7_configurations
 
 References
 ----------
-Please refer to the following for more detailed use: Nicholls, Z. R. J., Meinshausen, M., Lewis, J., Smith, C. J., Forster, P. M., Fuglestvedt, J. S., Rogelj, J., Kikstra, J. S., Riahi, K., and Byers, E.: Changes in IPCC scenario assessment emulators between SR1.5 and AR6 unravelled (*forthcoming*).
+Please refer to the following for more detailed use:
+
+  | Nicholls, Z. R. J., Meinshausen, M., Lewis, J., Smith, C. J., Forster, P. M., Fuglestvedt, J. S., Rogelj, J., Kikstra, J. S., Riahi, K., and Byers, E.
+  | "Changes in IPCC Scenario Assessment Emulators Between SR1.5 and AR6 Unraveled".
+  | *Geophysical Research Letters*
+  | https://doi.org/10.1029/2022GL099788
+  | 2022
 
 * More information, multiple references, and an interactive online tool: `magicc.org <https://magicc.org/>`_
 
 
 Advanced functionality
 ======================
 When running from the command line with CLI option ``--save-raw-climate-output``, an additional output folder will be created which writes out one large (~300-1000MB) file per scenario.
```

### Comparing `climate-assessment-0.1.1/doc/general.rst` & `climate-assessment-0.1.2/doc/general.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 .. _workflow:
 
 Description of the workflow
 ***************************
 On this page, you will find a short summary of the main function of this package.
-The workflow is described in detail in the following manuscript (exact citation TBD.):
+The workflow is described in detail in the following manuscript:
 
   | Jarmo S. Kikstra, Zebedee R. J. Nicholls, Christopher J. Smith, Jared Lewis, Robin D. Lamboll, Edward Byers, Marit Sandstad, Malte Meinshausen, Matthew J. Gidden, Joeri Rogelj, Elmar Kriegler, Glen P. Peters, Jan S. Fuglestvedt, Ragnhild B. Skeie, Bjørn H. Samset, Laura Wienpahl, Detlef P. van Vuuren, Kaj-Ivar van der Wijst, Alaa Al Khourdajie, Piers M. Forster, Andy Reisinger, Roberto Schaeffer, and Keywan Riahi
   | "The IPCC Sixth Assessment Report WGIII climate assessment of mitigation pathways: from emissions to global temperatures".
-  | *Geosci. Model Dev.*
-  | (in review)
+  | *Geosci. Model Dev., 15, 9075–9109*
+  | https://doi.org/10.5194/gmd-15-9075-2022
+  | 2022
 
 Integrated assessment models (IAMs) produce emissions pathways as part of larger pathway output coming from the modelling of scenarios.
 These emissions pathways imply a certain temperature development.
 
 Some integrated assessment modelling teams can provide their own climate model runs based on these emissions outcomes,
 others just work on the level of emissions.
 Not all IAMs model all societal processes that cause emissions and therefore not all models report pathways for all emissions species for all scenarios.
@@ -42,15 +43,16 @@
 `Step 1.` in AR6 was done by modelling teams across the world, with the scenarios submitted to and made available in the AR6 Scenario Database Explorer.
 
 `Step 2.`, `step 3.`, and `step 4`. are performed by this package.
 
 Expected Input (Step 1)
 =======================
 
-The expected input is in the following format, as either an Excel or CSV file, covering 2015, and then at minimum decadal (up to yearly detail is accepted) timesteps from 2020 to 2100.
+The expected input is in the following format, as either an Excel (.xlsx) or CSV (.csv) file, covering 2015, and then at minimum decadal (up to yearly detail is accepted) timesteps from 2020 to 2100.
+Currently, no meta data from the input data is used or preserved in the workflow.
 At minimum, one needs to report `Emissions|CO2|Energy and Industrial Processes`.
 Emissions baskets or species not in the table below are not considered for the eventual climate assessment, but are automatically infilled.
 In this version, negative values are only allowed as input for CO2.
 
 
 +--------+-----------+---------+------------------------------------------------+-----------------+-------+----+----+-------+
 | Model  | Scenario  | Region  | Variable                                       | Unit            | 2015  | …  | …  | 2100  |
```

### Comparing `climate-assessment-0.1.1/doc/index.rst` & `climate-assessment-0.1.2/doc/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -99,25 +99,25 @@
 .. _acknowledgements:
 
 Acknowledgements
 ================
 
 Per good scientific practice, you **must** cite the following publication when you use this package in scientific work.
 
-  | Jarmo S. Kikstra, Zebedee R. J. Nicholls, Christopher J. Smith, Jared Lewis, Robin D. Lamboll, Edward Byers, Marit Sanstad, Malte Meinshausen, Matthew J. Gidden, Joeri Rogelj, Elmar Kriegler, Glen P. Peters, Jan S. Fuglestvedt, Ragnhild B. Skeie, Bjørn H. Samset, Laura Wienpahl, Detlef P. van Vuuren, Kaj-Ivar van der Wijst, Alaa Al Khourdajie, Piers M. Forster, Andy Reisinger, Roberto Schaeffer, and Keywan Riahi
+  | Jarmo S. Kikstra, Zebedee R. J. Nicholls, Christopher J. Smith, Jared Lewis, Robin D. Lamboll, Edward Byers, Marit Sandstad, Malte Meinshausen, Matthew J. Gidden, Joeri Rogelj, Elmar Kriegler, Glen P. Peters, Jan S. Fuglestvedt, Ragnhild B. Skeie, Bjørn H. Samset, Laura Wienpahl, Detlef P. van Vuuren, Kaj-Ivar van der Wijst, Alaa Al Khourdajie, Piers M. Forster, Andy Reisinger, Roberto Schaeffer, and Keywan Riahi
   | "The IPCC Sixth Assessment Report WGIII climate assessment of mitigation pathways: from emissions to global temperatures".
-  | *Geosci. Model Dev.*
-  | (in review)
-
+  | *Geosci. Model Dev., 15, 9075–9109*
+  | https://doi.org/10.5194/gmd-15-9075-2022
+  | 2022
 
 You may additionally also cite the package itself:
 
   | Kikstra, J. S., Nicholls, Z. R. J., Lewis, J., Smith, C. J., Lamboll, R. D., Byers, E., Sandstad, M., Wienpahl, L., and Hackstock, P.:
-  | Climate assessment of long-term emissions pathways: IPCC AR6 WGIII version: Release v0.1.0,
-  | Zenodo, https://doi.org/10.5281/zenodo.6624520, 2022.
+  | Climate assessment of long-term emissions pathways: IPCC AR6 WGIII version,
+  | Zenodo, 10.5281/zenodo.6624519, 2022.
 
 
 For more detail, see :doc:`NOTICE`.
 
 .. toctree::
    :hidden:
    :caption: Acknowledgments
```

### Comparing `climate-assessment-0.1.1/doc/install.rst` & `climate-assessment-0.1.2/doc/install.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/make.bat` & `climate-assessment-0.1.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/prereqs.rst` & `climate-assessment-0.1.2/doc/prereqs.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/user_guide.rst` & `climate-assessment-0.1.2/doc/user_guide.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/doc/utility.rst` & `climate-assessment-0.1.2/doc/utility.rst`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/notebooks/run-example-ciceroscm.ipynb` & `climate-assessment-0.1.2/notebooks/run-example-ciceroscm.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/notebooks/run-example-custom.ipynb` & `climate-assessment-0.1.2/notebooks/run-example-custom.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/notebooks/run-example-fair.ipynb` & `climate-assessment-0.1.2/notebooks/run-example-fair.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/notebooks/run-example-magicc.ipynb` & `climate-assessment-0.1.2/notebooks/run-example-magicc.ipynb`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/scripts/generate-magicc-sr15-input-files.py` & `climate-assessment-0.1.2/scripts/generate-magicc-sr15-input-files.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/setup.cfg` & `climate-assessment-0.1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 keywords = climate, integrated assessment, emissions, temperature, IPCC
 description = Climate assessment of long-term emissions pathways: IPCC AR6 WGIII version
 long_description_content_type = text/x-rst
 long_description = file:README.rst
 url = https://github.com/iiasa/climate-assessment
 project_urls = 
 	Source = http://github.com/iiasa/climate-assessment
-	Documentation = https://iiasa-energy-program-climate-assessment.readthedocs-hosted.com/en/latest/
+	Documentation = https://climate-assessment.readthedocs.io/
 	Bug_Reports = https://github.com/iiasa/climate-assessment/issues
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
@@ -24,43 +24,43 @@
 [options]
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
 	aneris-iamc==0.3.1
-	awscli
+	awscli==1.27.134
 	click
 	fair==1.6.2
 	importlib-metadata
 	joblib
 	matplotlib
 	numpy
 	openscm-units==0.5.0
 	openscm-runner==0.9.1
 	pandas
-	pint>=0.13
+	pint>=0.13, <=0.20
 	pooch
-	pyam-iamc==1.4.0
+	pyam-iamc==1.7.0
 	pymagicc==2.1.3
 	requests
-	scmdata==0.14.0
-	silicone==1.2.1
+	scmdata==0.15.0
+	silicone==1.3.0
 	tqdm
 	xarray
 setup_requires = 
 	setuptools >= 41
 	setuptools_scm
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 docs = 
-	sphinx>=1.4
+	sphinx==5.3.0
 	sphinx_rtd_theme
 tests = 
 	codecov
 	nbval
 	pytest-cov
 	pytest-console-scripts
 	pytest>=4.0
```

### Comparing `climate-assessment-0.1.1/src/climate_assessment/__init__.py` & `climate-assessment-0.1.2/src/climate_assessment/__init__.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/checks.py` & `climate-assessment-0.1.2/src/climate_assessment/checks.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/cli.py` & `climate-assessment-0.1.2/src/climate_assessment/cli.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/climate/__init__.py` & `climate-assessment-0.1.2/src/climate_assessment/climate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         desc=f"{total_mod_scens} model-scenario pairs (running in batches of {scenario_batch_size})",
         total=total_mod_scens,
     ):
         batch_dfs.append(df)
         if np.equal((j + 1) % scenario_batch_size, 0) or np.equal(
             (j + 1), total_mod_scens
         ):
-            scenarios_to_run = pyam.concat(batch_dfs)
+            scenarios_to_run = pyam.IamDataFrame(pd.concat(batch_dfs))
 
             ##################################
             # run climate models
             ##################################
             _, res_percentiles, meta_table = run_and_post_process(
                 scenarios_to_run,
                 climate_model_cfgs,
@@ -250,15 +250,15 @@
         os.path.join(
             outdir,
             "{}_full_exceedance_probabilities.xlsx".format(key_string),
         )
     )
 
     LOGGER.info("Joining batches using pyam (slow as requires converting to long data)")
-    full_output = pyam.concat(full_output).data
+    full_output = pyam.IamDataFrame(pd.concat(full_output)).data
     # add prefix
     full_output["variable"] = prefix + "|" + full_output["variable"].astype(str)
     full_output = pyam.IamDataFrame(full_output)
 
     # include relevant meta in output
     meta_mod_scen = meta.set_index(["model", "scenario"])
     for c in meta_mod_scen:
```

### Comparing `climate-assessment-0.1.1/src/climate_assessment/climate/ciceroscm.py` & `climate-assessment-0.1.2/src/climate_assessment/climate/ciceroscm.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/climate/fair.py` & `climate-assessment-0.1.2/src/climate_assessment/climate/fair.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/climate/magicc7.py` & `climate-assessment-0.1.2/src/climate_assessment/climate/magicc7.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/climate/post_process.py` & `climate-assessment-0.1.2/src/climate_assessment/climate/post_process.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/climate/variable_definitions.csv` & `climate-assessment-0.1.2/src/climate_assessment/climate/variable_definitions.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/climate/wg3.py` & `climate-assessment-0.1.2/src/climate_assessment/climate/wg3.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/harmonization/__init__.py` & `climate-assessment-0.1.2/src/climate_assessment/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/harmonization/history_ar6.csv` & `climate-assessment-0.1.2/src/climate_assessment/harmonization/history_ar6.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/harmonization/history_sr15.csv` & `climate-assessment-0.1.2/src/climate_assessment/harmonization/history_sr15.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/harmonization_and_infilling.py` & `climate-assessment-0.1.2/src/climate_assessment/harmonization_and_infilling.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/infilling/__init__.py` & `climate-assessment-0.1.2/src/climate_assessment/infilling/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,14 @@
             LOGGER.info("Nothing to infill")
             continue
 
         LOGGER.info("Interpolating data to infill")
         to_infill = to_infill.interpolate(output_timesteps, inplace=False)
 
         if lead == ["Emissions|CO2"]:
-
             _, missing_energy = split_df(
                 to_infill, variable=f"{harmonized_prefix}|{co2_energy}"
             )
             if not missing_energy.empty:
                 # infill CO2 energy for scenarios that have CO2 total but no energy
 
                 if co2_afolu in missing_energy.variable:
```

### Comparing `climate-assessment-0.1.1/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv` & `climate-assessment-0.1.2/src/climate_assessment/infilling/cmip6-ssps-workflow-emissions.csv`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/postprocess.py` & `climate-assessment-0.1.2/src/climate_assessment/postprocess.py`

 * *Files identical despite different names*

### Comparing `climate-assessment-0.1.1/src/climate_assessment/testing.py` & `climate-assessment-0.1.2/src/climate_assessment/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,27 @@
     """
     pyam.iiasa.set_config(
         os.environ.get("SCENARIO_EXPLORER_USER"),
         os.environ.get("SCENARIO_EXPLORER_PASSWORD"),
         "iiasa_creds.yaml",
     )
     try:
-        conn = pyam.iiasa.Connection(
-            creds="iiasa_creds.yaml",
-            auth_url="https://db1.ene.iiasa.ac.at/EneAuth/config/v1",
-        )
+        conn = pyam.iiasa.Connection(creds="iiasa_creds.yaml")
     finally:
         # remove the yaml cred file
         os.remove("iiasa_creds.yaml")
 
     infiller_url = (
         "https://db1.ene.iiasa.ac.at/ar6-public-api/rest/v2.1/files/"
         f"{filename}?redirect=false"
     )
 
     return requests.get(
         infiller_url,
-        headers={"Authorization": f"Bearer {conn._token}"},
+        headers={"Authorization": f"Bearer {conn.auth.access_token}"},
     ).json()["directLink"]
 
 
 def _file_available_or_downloaded(filepath, hash_exp, url):
     """
     Check if file exists (and matches expected hash) or can be downloaded
```

### Comparing `climate-assessment-0.1.1/src/climate_assessment/utils.py` & `climate-assessment-0.1.2/src/climate_assessment/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import scmdata
 import tqdm.autonotebook as tqdman
 
 LOGGER = logging.getLogger(__name__)
 
 
 def init_logging(logger):
-
     # TODO: remove hard-coded level
     logger.setLevel(logging.INFO)
 
     # set root logger too
     logging.getLogger().setLevel(logging.INFO)
     logFormatter = logging.Formatter(
         "%(asctime)s %(name)s %(threadName)s - %(levelname)s:  %(message)s",
```

### Comparing `climate-assessment-0.1.1/src/climate_assessment.egg-info/PKG-INFO` & `climate-assessment-0.1.2/src/climate_assessment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: climate-assessment
-Version: 0.1.1
+Version: 0.1.2
 Summary: Climate assessment of long-term emissions pathways: IPCC AR6 WGIII version
 Home-page: https://github.com/iiasa/climate-assessment
 Author: Jarmo S. Kikstra, Zebedee R.J. Nicholls, Jared Lewis, Christopher J. Smith, Robin D. Lamboll, Edward Byers, Marit Sandstad, Laura Wienpahl, Philip Hackstock
 Author-email: kikstra@iiasa.ac.at
 License: MIT License
 Project-URL: Source, http://github.com/iiasa/climate-assessment
-Project-URL: Documentation, https://iiasa-energy-program-climate-assessment.readthedocs-hosted.com/en/latest/
+Project-URL: Documentation, https://climate-assessment.readthedocs.io/
 Project-URL: Bug_Reports, https://github.com/iiasa/climate-assessment/issues
 Keywords: climate,integrated assessment,emissions,temperature,IPCC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `climate-assessment-0.1.1/src/climate_assessment.egg-info/SOURCES.txt` & `climate-assessment-0.1.2/src/climate_assessment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

