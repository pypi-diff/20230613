# Comparing `tmp/tssm-0.0.2rc1.tar.gz` & `tmp/tssm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tssm-0.0.2rc1.tar", last modified: Tue Aug  9 12:51:32 2022, max compression
+gzip compressed data, was "tssm-0.0.4.tar", last modified: Tue Jun 13 14:20:56 2023, max compression
```

## Comparing `tssm-0.0.2rc1.tar` & `tssm-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-08-09 12:51:32.218798 tssm-0.0.2rc1/
--rw-rw-rw-   0        0        0     1550 2022-08-01 07:30:33.000000 tssm-0.0.2rc1/LICENSE
--rw-rw-rw-   0        0        0     6807 2022-08-09 12:51:32.219796 tssm-0.0.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0     5773 2022-08-09 12:44:45.000000 tssm-0.0.2rc1/README.md
--rw-rw-rw-   0        0        0      577 2022-08-09 12:15:00.000000 tssm-0.0.2rc1/pyproject.toml
--rw-rw-rw-   0        0        0     1331 2022-08-09 12:51:32.220795 tssm-0.0.2rc1/setup.cfg
--rw-rw-rw-   0        0        0      573 2022-08-01 08:47:52.000000 tssm-0.0.2rc1/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-09 12:51:32.214795 tssm-0.0.2rc1/tssm/
--rw-rw-rw-   0        0        0      126 2022-08-09 12:03:18.000000 tssm-0.0.2rc1/tssm/__init__.py
--rw-rw-rw-   0        0        0    20593 2022-08-09 12:03:18.000000 tssm-0.0.2rc1/tssm/time_series_scaling_module.py
--rw-rw-rw-   0        0        0    10690 2022-08-08 07:30:09.000000 tssm-0.0.2rc1/tssm/value_storage.py
-drwxrwxrwx   0        0        0        0 2022-08-09 12:51:32.218798 tssm-0.0.2rc1/tssm.egg-info/
--rw-rw-rw-   0        0        0     6807 2022-08-09 12:51:32.000000 tssm-0.0.2rc1/tssm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2022-08-09 12:51:32.000000 tssm-0.0.2rc1/tssm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-09 12:51:32.000000 tssm-0.0.2rc1/tssm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-09 12:16:42.000000 tssm-0.0.2rc1/tssm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      179 2022-08-09 12:51:32.000000 tssm-0.0.2rc1/tssm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-08-09 12:51:32.000000 tssm-0.0.2rc1/tssm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.981469 tssm-0.0.4/
+-rw-rw-rw-   0        0        0     1550 2022-08-01 07:30:33.000000 tssm-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6254 2023-06-13 14:20:56.981725 tssm-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5223 2023-03-22 09:54:26.000000 tssm-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1496 2023-03-22 09:54:26.000000 tssm-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1349 2023-06-13 14:20:56.982469 tssm-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      573 2022-08-31 11:04:49.000000 tssm-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.902703 tssm-0.0.4/tests/
+-rw-rw-rw-   0        0        0     3013 2023-06-13 13:49:53.000000 tssm-0.0.4/tests/test_bdew_electrical.py
+-rw-rw-rw-   0        0        0     1565 2023-06-13 13:49:53.000000 tssm-0.0.4/tests/test_bdew_heat.py
+-rw-rw-rw-   0        0        0     8290 2023-03-22 09:54:26.000000 tssm-0.0.4/tests/test_data_import.py
+-rw-rw-rw-   0        0        0     2508 2023-06-13 13:49:57.000000 tssm-0.0.4/tests/test_date_format_check.py
+-rw-rw-rw-   0        0        0     2690 2023-06-13 13:47:13.000000 tssm-0.0.4/tests/test_export.py
+-rw-rw-rw-   0        0        0    10188 2023-06-13 13:49:57.000000 tssm-0.0.4/tests/test_given_simultaneity_factor.py
+-rw-rw-rw-   0        0        0     5791 2023-06-13 13:49:57.000000 tssm-0.0.4/tests/test_index_and_average.py
+-rw-rw-rw-   0        0        0    12849 2023-06-13 13:49:57.000000 tssm-0.0.4/tests/test_linear.py
+-rw-rw-rw-   0        0        0    18690 2023-06-13 13:49:57.000000 tssm-0.0.4/tests/test_normal_distribution.py
+-rw-rw-rw-   0        0        0     4031 2023-04-19 12:31:02.000000 tssm-0.0.4/tests/test_scaling_normal_distribution.py
+-rw-rw-rw-   0        0        0    22436 2023-06-13 13:49:57.000000 tssm-0.0.4/tests/test_scaling_profile.py
+-rw-rw-rw-   0        0        0     1793 2023-06-13 13:49:57.000000 tssm-0.0.4/tests/test_simultaneity_factor_calculation.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.904704 tssm-0.0.4/tssm/
+-rw-rw-rw-   0        0        0      432 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.938353 tssm-0.0.4/tssm/calculation_models/
+-rw-rw-rw-   0        0        0      633 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/__init__.py
+-rw-rw-rw-   0        0        0     5215 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/average_calculation_model.py
+-rw-rw-rw-   0        0        0     1782 2023-03-23 06:11:32.000000 tssm-0.0.4/tssm/calculation_models/calculation_base_class.py
+-rw-rw-rw-   0        0        0      299 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/maximum_class.py
+-rw-rw-rw-   0        0        0    14468 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/normal_distribution_model.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.943026 tssm-0.0.4/tssm/calculation_models/profile_generation/
+-rw-rw-rw-   0        0        0      194 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/profile_generation/__init__.py
+-rw-rw-rw-   0        0        0     4210 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/profile_generation/bdew_electrical.py
+-rw-rw-rw-   0        0        0    17016 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/profile_generation/bdew_heat.py
+-rw-rw-rw-   0        0        0     3223 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/profile_generation/functions.py
+-rw-rw-rw-   0        0        0   558765 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/profile_generation/hour_dict.py
+-rw-rw-rw-   0        0        0     3107 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/scaling_and_normal_distribution_model.py
+-rw-rw-rw-   0        0        0     7118 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/scaling_profile_model.py
+-rw-rw-rw-   0        0        0     1368 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/calculation_models/simultaneity_factor.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.970932 tssm-0.0.4/tssm/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:47:13.000000 tssm-0.0.4/tssm/gui/__init__.py
+-rw-rw-rw-   0        0        0      272 2023-06-13 13:47:13.000000 tssm-0.0.4/tssm/gui/create_translation_class.py
+-rw-rw-rw-   0        0        0     1457 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/gui/data_2_tssm.py
+-rw-rw-rw-   0        0        0    12984 2023-06-13 14:09:38.000000 tssm-0.0.4/tssm/gui/gui_structure.py
+-rw-rw-rw-   0        0        0     5697 2023-06-13 14:05:04.000000 tssm-0.0.4/tssm/gui/start_gui.py
+-rw-rw-rw-   0        0        0    12784 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/gui/translation_class.py
+-rw-rw-rw-   0        0        0     8288 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/time_series_scaling_module.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.980361 tssm-0.0.4/tssm/utils/
+-rw-rw-rw-   0        0        0   306076 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/BDEW_class.py
+-rw-rw-rw-   0        0        0      212 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/BDEW_day.py
+-rw-rw-rw-   0        0        0      391 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/__init__.py
+-rw-rw-rw-   0        0        0     2466 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/calc_indexes.py
+-rw-rw-rw-   0        0        0     1672 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/cast_2_same_sum.py
+-rw-rw-rw-   0        0        0     1235 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/cast_input_2_period.py
+-rw-rw-rw-   0        0        0     1496 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/create_bdew_electrical_data_class.py
+-rw-rw-rw-   0        0        0     4747 2023-06-13 13:47:13.000000 tssm-0.0.4/tssm/utils/dict_casting.py
+-rw-rw-rw-   0        0        0      444 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/errors.py
+-rw-rw-rw-   0        0        0      295 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/period.py
+-rw-rw-rw-   0        0        0      190 2023-06-13 13:49:57.000000 tssm-0.0.4/tssm/utils/seasons.py
+-rw-rw-rw-   0        0        0    11984 2023-06-13 13:47:13.000000 tssm-0.0.4/tssm/value_storage.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:20:56.909508 tssm-0.0.4/tssm.egg-info/
+-rw-rw-rw-   0        0        0     6254 2023-06-13 14:20:56.000000 tssm-0.0.4/tssm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-06-13 14:20:56.000000 tssm-0.0.4/tssm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:20:56.000000 tssm-0.0.4/tssm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-09 12:16:42.000000 tssm-0.0.4/tssm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      261 2023-06-13 14:20:56.000000 tssm-0.0.4/tssm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 14:20:56.000000 tssm-0.0.4/tssm.egg-info/top_level.txt
```

### Comparing `tssm-0.0.2rc1/LICENSE` & `tssm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tssm-0.0.2rc1/PKG-INFO` & `tssm-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tssm
-Version: 0.0.2rc1
+Version: 0.0.4
 Summary: Package to create out of a single load profile a profile for a whole district using the diversity factor
 Home-page: https://git.fh-aachen.de/tb5152e/tssm
 Author: Tobias Blanke & Dominik Fischer
 License: BSD 3-Clause License
 Keywords: load,simultaneity factor,scaling,load profile,time series
 Platform: unix
 Platform: linux
@@ -26,74 +26,77 @@
 License-File: LICENSE
 
 [![Status](https://img.shields.io/pypi/status/tssm)](https://pypi.python.org/pypi/tssm)
 [![Version](https://img.shields.io/pypi/v/tssm.svg)](https://pypi.python.org/pypi/tssm)
 [![Python Version](https://img.shields.io/pypi/pyversions/tssm)](https://pypi.python.org/pypi/tssm)
 [![Wheel](https://img.shields.io/pypi/wheel/tssm)](https://pypi.python.org/pypi/tssm)
 [![PyPI - License](https://img.shields.io/pypi/l/tssm)](https://opensource.org/licenses/BSD-3-Clause)
+
+[![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases)
+[![OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/issues)
+
 [![Documentation Status](https://readthedocs.org/projects/tssm/badge/?version=latest)](https://tssm.readthedocs.io/en/latest/?badge=latest)
-[![coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
 [![pipeline status](https://git.fh-aachen.de/tb5152e/tssm/badges/main/pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases)
-[![Pylint](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/pylint.svg?job=pylint)](https://pylint.pycqa.org/en/latest/)
+[![coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Pylint](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/pylint.svg&job=pylint)](https://pylint.pycqa.org/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](http://mypy-lang.org/)
 [![security: bandit](https://img.shields.io/badge/security-bandit-success.svg)](https://github.com/PyCQA/bandit)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/issues)
 
 
-<a href="https://www.fh-aachen.de/forschung/solar-institut-juelich"><img src="https://www.fh-aachen.de/fileadmin/ins/ins_sij/Wortmarke_SIJ_ts_web.jpg" alt="Forschungszentrum Juelich Logo"></a> 
+<a href="https://www.fh-aachen.de/forschung/solar-institut-juelich"><img src="https://www.fh-aachen.de/fileadmin/ins/ins_sij/Wortmarke_SIJ_ts_web.jpg" 
+alt="Solar Institute Juelich Logo"></a> 
 
 # Time Series Scaling Module  (TSSM)
-TSSM is a python package for the scaling of time series. 
+<img src="./docs/sources/_static/Logo.svg" width="100" align="left">
+
+**TSSM** is a python package for the up-scaling of time series or load such as electricity, heating, etc. 
+
 
 **Warning**
 ```{warning} 
 This package is under heavy development!
 ```
 
 ## Getting started
-### Install tssm
-Install tssm directly from PyPi as follows. It is recommended to set up a fresh Conda environment before using this package by following these steps:
 
-* Install Miniconda or update your conda installation with `conda update conda`
-* Create a new environment with `conda create -n <environmentName> python=<pythonVersion>`. The python version to be specified should be greater than python 3.8. 
-* Activate the environment with `source activate <environmentName>` on Linux/MacOS or `activate <environmentName>` on Windows
-* Clone tssm with `git clone https://git.fh-aachen.de/tb5152e/tssm.git`
-* Install tssm with `pip install -e <path_to_tssm_package>`
-* Verify your tssm package installtion by running the configured automated tests. Go to your tssm top-level directory and type `pytest`
+### Install TSSM
+
+Install tssm directly from PyPi as follows: 
 
-Or you can also directly install tssm package from PyPi with the following command
 ```console
 pip install tssm
 ```
 
+Further installation instructions can be found in the [**documentation**](http://tssm.rtfd.io/) under 'Getting started'.
+
+
 ### Usage
 
 example usages can be found in the [**examples'**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples) folder.
 
 
 #### Basic workflow
 
 A small example how tssm can be used is described as follows:
 
 ```python
-# import module
-from tssm import TimeSeriesScalingModule as tssm
+# import module and Daily period variable
+from tssm import TimeSeriesScalingModule as tssm, DAILY
 
 # initialize class with a number of buildings of 202 with a simultaneity factor of 0.786
-df_test = tssm(number_of_buildings=202, simultaneity_factor=0.786)
+scaling = tssm(number_of_buildings=202, simultaneity_factor=0.786)
 # read profile from data.csv file and use the Electricity and Date column
-df_test.values.read_profile_from_csv_with_date(path="./data.csv", column_of_load="Electricity", column_of_date="Date")
-# calculate linear scaled values with a daily (period=1) simultaneity factor and average value
-daily_scaled_values = df_test.calculate_linear(period=1)
+scaling.data.read_profile_from_csv_with_date(path="./data.csv", column_of_load="Electricity", column_of_date="Date")
+# calculate linear scaled values with a daily simultaneity factor and average value
+daily_scaled_values = scaling.calculate_using_average_values(period=DAILY)
 ```
 
 #### Examples
 A [**first example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/example_linear.py) shows the linear approach. It scales the time series between the scaled time series and an average.
 
 A [**second example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/example_scaling.py) shows the scaling approach. It scales the time series between the scaled time series and a scaling time 
 series.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tssm Version: 0.0.2rc1 Summary: Package to create
-out of a single load profile a profile for a whole district using the diversity
+Metadata-Version: 2.1 Name: tssm Version: 0.0.4 Summary: Package to create out
+of a single load profile a profile for a whole district using the diversity
 factor Home-page: https://git.fh-aachen.de/tb5152e/tssm Author: Tobias Blanke &
 Dominik Fischer License: BSD 3-Clause License Keywords: load,simultaneity
 factor,scaling,load profile,time series Platform: unix Platform: linux
 Platform: osx Platform: win32 Platform: win64 Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Development Status :: 3 -
 Alpha Classifier: License :: OSI Approved :: BSD License Classifier: Intended
@@ -13,74 +13,67 @@
 Description-Content-Type: text/markdown Provides-Extra: testing License-File:
 LICENSE [![Status](https://img.shields.io/pypi/status/tssm)](https://
 pypi.python.org/pypi/tssm) [![Version](https://img.shields.io/pypi/v/tssm.svg)]
 (https://pypi.python.org/pypi/tssm) [![Python Version](https://img.shields.io/
 pypi/pyversions/tssm)](https://pypi.python.org/pypi/tssm) [![Wheel](https://
 img.shields.io/pypi/wheel/tssm)](https://pypi.python.org/pypi/tssm) [![PyPI -
 License](https://img.shields.io/pypi/l/tssm)](https://opensource.org/licenses/
-BSD-3-Clause) [![Documentation Status](https://readthedocs.org/projects/tssm/
+BSD-3-Clause) [![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/
+artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-
+aachen.de/tb5152e/tssm/-/commits/main) [![Last Release](https://git.fh-
+aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/
+last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/
+main) [![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/
+release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases) [!
+[OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/
+public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/
+tssm/-/issues) [![Documentation Status](https://readthedocs.org/projects/tssm/
 badge/?version=latest)](https://tssm.readthedocs.io/en/latest/?badge=latest) [!
-[coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
-coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [!
 [pipeline status](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
-pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [![Latest
-Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://
-git.fh-aachen.de/tb5152e/diversityfactor/-/releases) [![Pylint](https://git.fh-
-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/
-pylint.svg?job=pylint)](https://pylint.pycqa.org/en/latest/) [![Code style:
+pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [!
+[coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
+coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [![Pylint]
+(https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/
+pylint.svg&job=pylint)](https://pylint.pycqa.org/en/latest/) [![Code style:
 black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/
-%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
-pycqa.github.io/isort/) [![Checked with mypy](http://www.mypy-lang.org/static/
-mypy_badge.svg)](http://mypy-lang.org/) [![security: bandit](https://
-img.shields.io/badge/security-bandit-success.svg)](https://github.com/PyCQA/
-bandit) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-
-1f425f.svg)](https://www.python.org/) [![Last Commit](https://git.fh-aachen.de/
-tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/
-last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/
-main) [![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/
-main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/
-tb5152e/tssm/-/commits/main) [![OpenIssues](https://git.fh-aachen.de/tb5152e/
-tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)]
-(https://git.fh-aachen.de/tb5152e/tssm/-/issues) [Forschungszentrum_Juelich
-Logo] # Time Series Scaling Module (TSSM) TSSM is a python package for the
-scaling of time series. **Warning** ```{warning} This package is under heavy
-development! ``` ## Getting started ### Install tssm Install tssm directly from
-PyPi as follows. It is recommended to set up a fresh Conda environment before
-using this package by following these steps: * Install Miniconda or update your
-conda installation with `conda update conda` * Create a new environment with
-`conda create -n  python=`. The python version to be specified should be
-greater than python 3.8. * Activate the environment with `source activate ` on
-Linux/MacOS or `activate ` on Windows * Clone tssm with `git clone https://
-git.fh-aachen.de/tb5152e/tssm.git` * Install tssm with `pip install -e ` *
-Verify your tssm package installtion by running the configured automated tests.
-Go to your tssm top-level directory and type `pytest` Or you can also directly
-install tssm package from PyPi with the following command ```console pip
-install tssm ``` ### Usage example usages can be found in the [**examples'**]
-(https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples) folder. #### Basic
-workflow A small example how tssm can be used is described as follows:
-```python # import module from tssm import TimeSeriesScalingModule as tssm #
-initialize class with a number of buildings of 202 with a simultaneity factor
-of 0.786 df_test = tssm(number_of_buildings=202, simultaneity_factor=0.786) #
-read profile from data.csv file and use the Electricity and Date column
-df_test.values.read_profile_from_csv_with_date(path="./data.csv",
-column_of_load="Electricity", column_of_date="Date") # calculate linear scaled
-values with a daily (period=1) simultaneity factor and average value
-daily_scaled_values = df_test.calculate_linear(period=1) ``` #### Examples A
-[**first example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/
-example_linear.py) shows the linear approach. It scales the time series between
-the scaled time series and an average. A [**second example**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/examples/example_scaling.py) shows the
-scaling approach. It scales the time series between the scaled time series and
-a scaling time series. A [**third example**](https://git.fh-aachen.de/tb5152e/
-tssm/-/blob/main/examples/example_normal_distribution.py) shows the normal
-distribution approach. It scales the time series by applying a normal
-distribution to every time step. A [**fourth example**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/examples/
-example_of_different_method_2_import_profiles.py) shows the different ways to
-import the data. A [**fifth example**](https://git.fh-aachen.de/tb5152e/tssm/-/
-blob/main/examples/example_speed_comparison.py) shows the speed of the
-different approaches. ### License The module is licensed under BSD 3-Clause
-License. Further, License information can be found [**here**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/LICENSE). ### Reference ### Acknowledgements
-## Content The documentation of the tssm code can be found [**here**](http://
-tssm.rtfd.io/).
+%20imports-isort-%231674b1&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](http://
+mypy-lang.org/) [![security: bandit](https://img.shields.io/badge/security-
+bandit-success.svg)](https://github.com/PyCQA/bandit) [![made-with-python]
+(https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://
+www.python.org/) [Solar_Institute_Juelich_Logo] # Time Series Scaling Module
+(TSSM) [./docs/sources/_static/Logo.svg] **TSSM** is a python package for the
+up-scaling of time series or load such as electricity, heating, etc.
+**Warning** ```{warning} This package is under heavy development! ``` ##
+Getting started ### Install TSSM Install tssm directly from PyPi as follows:
+```console pip install tssm ``` Further installation instructions can be found
+in the [**documentation**](http://tssm.rtfd.io/) under 'Getting started'. ###
+Usage example usages can be found in the [**examples'**](https://git.fh-
+aachen.de/tb5152e/tssm/-/blob/main/examples) folder. #### Basic workflow A
+small example how tssm can be used is described as follows: ```python # import
+module and Daily period variable from tssm import TimeSeriesScalingModule as
+tssm, DAILY # initialize class with a number of buildings of 202 with a
+simultaneity factor of 0.786 scaling = tssm(number_of_buildings=202,
+simultaneity_factor=0.786) # read profile from data.csv file and use the
+Electricity and Date column scaling.data.read_profile_from_csv_with_date
+(path="./data.csv", column_of_load="Electricity", column_of_date="Date") #
+calculate linear scaled values with a daily simultaneity factor and average
+value daily_scaled_values = scaling.calculate_using_average_values
+(period=DAILY) ``` #### Examples A [**first example**](https://git.fh-
+aachen.de/tb5152e/tssm/-/blob/main/examples/example_linear.py) shows the linear
+approach. It scales the time series between the scaled time series and an
+average. A [**second example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/
+main/examples/example_scaling.py) shows the scaling approach. It scales the
+time series between the scaled time series and a scaling time series. A
+[**third example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/
+example_normal_distribution.py) shows the normal distribution approach. It
+scales the time series by applying a normal distribution to every time step. A
+[**fourth example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/
+examples/example_of_different_method_2_import_profiles.py) shows the different
+ways to import the data. A [**fifth example**](https://git.fh-aachen.de/
+tb5152e/tssm/-/blob/main/examples/example_speed_comparison.py) shows the speed
+of the different approaches. ### License The module is licensed under BSD 3-
+Clause License. Further, License information can be found [**here**](https://
+git.fh-aachen.de/tb5152e/tssm/-/blob/main/LICENSE). ### Reference ###
+Acknowledgements ## Content The documentation of the tssm code can be found
+[**here**](http://tssm.rtfd.io/).
```

### Comparing `tssm-0.0.2rc1/README.md` & `tssm-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 [![Status](https://img.shields.io/pypi/status/tssm)](https://pypi.python.org/pypi/tssm)
 [![Version](https://img.shields.io/pypi/v/tssm.svg)](https://pypi.python.org/pypi/tssm)
 [![Python Version](https://img.shields.io/pypi/pyversions/tssm)](https://pypi.python.org/pypi/tssm)
 [![Wheel](https://img.shields.io/pypi/wheel/tssm)](https://pypi.python.org/pypi/tssm)
 [![PyPI - License](https://img.shields.io/pypi/l/tssm)](https://opensource.org/licenses/BSD-3-Clause)
+
+[![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases)
+[![OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/issues)
+
 [![Documentation Status](https://readthedocs.org/projects/tssm/badge/?version=latest)](https://tssm.readthedocs.io/en/latest/?badge=latest)
-[![coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
 [![pipeline status](https://git.fh-aachen.de/tb5152e/tssm/badges/main/pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases)
-[![Pylint](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/pylint.svg?job=pylint)](https://pylint.pycqa.org/en/latest/)
+[![coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Pylint](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/pylint.svg&job=pylint)](https://pylint.pycqa.org/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](http://mypy-lang.org/)
 [![security: bandit](https://img.shields.io/badge/security-bandit-success.svg)](https://github.com/PyCQA/bandit)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/issues)
 
 
-<a href="https://www.fh-aachen.de/forschung/solar-institut-juelich"><img src="https://www.fh-aachen.de/fileadmin/ins/ins_sij/Wortmarke_SIJ_ts_web.jpg" alt="Forschungszentrum Juelich Logo"></a> 
+<a href="https://www.fh-aachen.de/forschung/solar-institut-juelich"><img src="https://www.fh-aachen.de/fileadmin/ins/ins_sij/Wortmarke_SIJ_ts_web.jpg" 
+alt="Solar Institute Juelich Logo"></a> 
 
 # Time Series Scaling Module  (TSSM)
-TSSM is a python package for the scaling of time series. 
+<img src="./docs/sources/_static/Logo.svg" width="100" align="left">
+
+**TSSM** is a python package for the up-scaling of time series or load such as electricity, heating, etc. 
+
 
 **Warning**
 ```{warning} 
 This package is under heavy development!
 ```
 
 ## Getting started
-### Install tssm
-Install tssm directly from PyPi as follows. It is recommended to set up a fresh Conda environment before using this package by following these steps:
 
-* Install Miniconda or update your conda installation with `conda update conda`
-* Create a new environment with `conda create -n <environmentName> python=<pythonVersion>`. The python version to be specified should be greater than python 3.8. 
-* Activate the environment with `source activate <environmentName>` on Linux/MacOS or `activate <environmentName>` on Windows
-* Clone tssm with `git clone https://git.fh-aachen.de/tb5152e/tssm.git`
-* Install tssm with `pip install -e <path_to_tssm_package>`
-* Verify your tssm package installtion by running the configured automated tests. Go to your tssm top-level directory and type `pytest`
+### Install TSSM
+
+Install tssm directly from PyPi as follows: 
 
-Or you can also directly install tssm package from PyPi with the following command
 ```console
 pip install tssm
 ```
 
+Further installation instructions can be found in the [**documentation**](http://tssm.rtfd.io/) under 'Getting started'.
+
+
 ### Usage
 
 example usages can be found in the [**examples'**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples) folder.
 
 
 #### Basic workflow
 
 A small example how tssm can be used is described as follows:
 
 ```python
-# import module
-from tssm import TimeSeriesScalingModule as tssm
+# import module and Daily period variable
+from tssm import TimeSeriesScalingModule as tssm, DAILY
 
 # initialize class with a number of buildings of 202 with a simultaneity factor of 0.786
-df_test = tssm(number_of_buildings=202, simultaneity_factor=0.786)
+scaling = tssm(number_of_buildings=202, simultaneity_factor=0.786)
 # read profile from data.csv file and use the Electricity and Date column
-df_test.values.read_profile_from_csv_with_date(path="./data.csv", column_of_load="Electricity", column_of_date="Date")
-# calculate linear scaled values with a daily (period=1) simultaneity factor and average value
-daily_scaled_values = df_test.calculate_linear(period=1)
+scaling.data.read_profile_from_csv_with_date(path="./data.csv", column_of_load="Electricity", column_of_date="Date")
+# calculate linear scaled values with a daily simultaneity factor and average value
+daily_scaled_values = scaling.calculate_using_average_values(period=DAILY)
 ```
 
 #### Examples
 A [**first example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/example_linear.py) shows the linear approach. It scales the time series between the scaled time series and an average.
 
 A [**second example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/example_scaling.py) shows the scaling approach. It scales the time series between the scaled time series and a scaling time 
 series.
```

#### html2text {}

```diff
@@ -1,73 +1,66 @@
 [![Status](https://img.shields.io/pypi/status/tssm)](https://pypi.python.org/
 pypi/tssm) [![Version](https://img.shields.io/pypi/v/tssm.svg)](https://
 pypi.python.org/pypi/tssm) [![Python Version](https://img.shields.io/pypi/
 pyversions/tssm)](https://pypi.python.org/pypi/tssm) [![Wheel](https://
 img.shields.io/pypi/wheel/tssm)](https://pypi.python.org/pypi/tssm) [![PyPI -
 License](https://img.shields.io/pypi/l/tssm)](https://opensource.org/licenses/
-BSD-3-Clause) [![Documentation Status](https://readthedocs.org/projects/tssm/
+BSD-3-Clause) [![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/
+artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-
+aachen.de/tb5152e/tssm/-/commits/main) [![Last Release](https://git.fh-
+aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/
+last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/
+main) [![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/
+release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases) [!
+[OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/
+public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/
+tssm/-/issues) [![Documentation Status](https://readthedocs.org/projects/tssm/
 badge/?version=latest)](https://tssm.readthedocs.io/en/latest/?badge=latest) [!
-[coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
-coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [!
 [pipeline status](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
-pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [![Latest
-Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://
-git.fh-aachen.de/tb5152e/diversityfactor/-/releases) [![Pylint](https://git.fh-
-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/
-pylint.svg?job=pylint)](https://pylint.pycqa.org/en/latest/) [![Code style:
+pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [!
+[coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
+coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [![Pylint]
+(https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/
+pylint.svg&job=pylint)](https://pylint.pycqa.org/en/latest/) [![Code style:
 black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/
-%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
-pycqa.github.io/isort/) [![Checked with mypy](http://www.mypy-lang.org/static/
-mypy_badge.svg)](http://mypy-lang.org/) [![security: bandit](https://
-img.shields.io/badge/security-bandit-success.svg)](https://github.com/PyCQA/
-bandit) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-
-1f425f.svg)](https://www.python.org/) [![Last Commit](https://git.fh-aachen.de/
-tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/
-last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/
-main) [![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/
-main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/
-tb5152e/tssm/-/commits/main) [![OpenIssues](https://git.fh-aachen.de/tb5152e/
-tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)]
-(https://git.fh-aachen.de/tb5152e/tssm/-/issues) [Forschungszentrum_Juelich
-Logo] # Time Series Scaling Module (TSSM) TSSM is a python package for the
-scaling of time series. **Warning** ```{warning} This package is under heavy
-development! ``` ## Getting started ### Install tssm Install tssm directly from
-PyPi as follows. It is recommended to set up a fresh Conda environment before
-using this package by following these steps: * Install Miniconda or update your
-conda installation with `conda update conda` * Create a new environment with
-`conda create -n  python=`. The python version to be specified should be
-greater than python 3.8. * Activate the environment with `source activate ` on
-Linux/MacOS or `activate ` on Windows * Clone tssm with `git clone https://
-git.fh-aachen.de/tb5152e/tssm.git` * Install tssm with `pip install -e ` *
-Verify your tssm package installtion by running the configured automated tests.
-Go to your tssm top-level directory and type `pytest` Or you can also directly
-install tssm package from PyPi with the following command ```console pip
-install tssm ``` ### Usage example usages can be found in the [**examples'**]
-(https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples) folder. #### Basic
-workflow A small example how tssm can be used is described as follows:
-```python # import module from tssm import TimeSeriesScalingModule as tssm #
-initialize class with a number of buildings of 202 with a simultaneity factor
-of 0.786 df_test = tssm(number_of_buildings=202, simultaneity_factor=0.786) #
-read profile from data.csv file and use the Electricity and Date column
-df_test.values.read_profile_from_csv_with_date(path="./data.csv",
-column_of_load="Electricity", column_of_date="Date") # calculate linear scaled
-values with a daily (period=1) simultaneity factor and average value
-daily_scaled_values = df_test.calculate_linear(period=1) ``` #### Examples A
-[**first example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/
-example_linear.py) shows the linear approach. It scales the time series between
-the scaled time series and an average. A [**second example**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/examples/example_scaling.py) shows the
-scaling approach. It scales the time series between the scaled time series and
-a scaling time series. A [**third example**](https://git.fh-aachen.de/tb5152e/
-tssm/-/blob/main/examples/example_normal_distribution.py) shows the normal
-distribution approach. It scales the time series by applying a normal
-distribution to every time step. A [**fourth example**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/examples/
-example_of_different_method_2_import_profiles.py) shows the different ways to
-import the data. A [**fifth example**](https://git.fh-aachen.de/tb5152e/tssm/-/
-blob/main/examples/example_speed_comparison.py) shows the speed of the
-different approaches. ### License The module is licensed under BSD 3-Clause
-License. Further, License information can be found [**here**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/LICENSE). ### Reference ### Acknowledgements
-## Content The documentation of the tssm code can be found [**here**](http://
-tssm.rtfd.io/).
+%20imports-isort-%231674b1&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](http://
+mypy-lang.org/) [![security: bandit](https://img.shields.io/badge/security-
+bandit-success.svg)](https://github.com/PyCQA/bandit) [![made-with-python]
+(https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://
+www.python.org/) [Solar_Institute_Juelich_Logo] # Time Series Scaling Module
+(TSSM) [./docs/sources/_static/Logo.svg] **TSSM** is a python package for the
+up-scaling of time series or load such as electricity, heating, etc.
+**Warning** ```{warning} This package is under heavy development! ``` ##
+Getting started ### Install TSSM Install tssm directly from PyPi as follows:
+```console pip install tssm ``` Further installation instructions can be found
+in the [**documentation**](http://tssm.rtfd.io/) under 'Getting started'. ###
+Usage example usages can be found in the [**examples'**](https://git.fh-
+aachen.de/tb5152e/tssm/-/blob/main/examples) folder. #### Basic workflow A
+small example how tssm can be used is described as follows: ```python # import
+module and Daily period variable from tssm import TimeSeriesScalingModule as
+tssm, DAILY # initialize class with a number of buildings of 202 with a
+simultaneity factor of 0.786 scaling = tssm(number_of_buildings=202,
+simultaneity_factor=0.786) # read profile from data.csv file and use the
+Electricity and Date column scaling.data.read_profile_from_csv_with_date
+(path="./data.csv", column_of_load="Electricity", column_of_date="Date") #
+calculate linear scaled values with a daily simultaneity factor and average
+value daily_scaled_values = scaling.calculate_using_average_values
+(period=DAILY) ``` #### Examples A [**first example**](https://git.fh-
+aachen.de/tb5152e/tssm/-/blob/main/examples/example_linear.py) shows the linear
+approach. It scales the time series between the scaled time series and an
+average. A [**second example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/
+main/examples/example_scaling.py) shows the scaling approach. It scales the
+time series between the scaled time series and a scaling time series. A
+[**third example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/
+example_normal_distribution.py) shows the normal distribution approach. It
+scales the time series by applying a normal distribution to every time step. A
+[**fourth example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/
+examples/example_of_different_method_2_import_profiles.py) shows the different
+ways to import the data. A [**fifth example**](https://git.fh-aachen.de/
+tb5152e/tssm/-/blob/main/examples/example_speed_comparison.py) shows the speed
+of the different approaches. ### License The module is licensed under BSD 3-
+Clause License. Further, License information can be found [**here**](https://
+git.fh-aachen.de/tb5152e/tssm/-/blob/main/LICENSE). ### Reference ###
+Acknowledgements ## Content The documentation of the tssm code can be found
+[**here**](http://tssm.rtfd.io/).
```

### Comparing `tssm-0.0.2rc1/setup.cfg` & `tssm-0.0.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7373 6d0d 0a76 6572 7369 6f6e   = tssm..version
-00000020: 203d 2030 2e30 2e32 2d70 7265 310d 0a61   = 0.0.2-pre1..a
-00000030: 7574 686f 7220 3d20 546f 6269 6173 2042  uthor = Tobias B
-00000040: 6c61 6e6b 6520 2620 446f 6d69 6e69 6b20  lanke & Dominik 
-00000050: 4669 7363 6865 720d 0a64 6573 6372 6970  Fischer..descrip
-00000060: 7469 6f6e 203d 2050 6163 6b61 6765 2074  tion = Package t
-00000070: 6f20 6372 6561 7465 206f 7574 206f 6620  o create out of 
-00000080: 6120 7369 6e67 6c65 206c 6f61 6420 7072  a single load pr
-00000090: 6f66 696c 6520 6120 7072 6f66 696c 6520  ofile a profile 
-000000a0: 666f 7220 6120 7768 6f6c 6520 6469 7374  for a whole dist
-000000b0: 7269 6374 2075 7369 6e67 2074 6865 2064  rict using the d
-000000c0: 6976 6572 7369 7479 2066 6163 746f 720d  iversity factor.
-000000d0: 0a6b 6579 776f 7264 7320 3d20 6c6f 6164  .keywords = load
-000000e0: 2c20 7369 6d75 6c74 616e 6569 7479 2066  , simultaneity f
-000000f0: 6163 746f 722c 2073 6361 6c69 6e67 2c20  actor, scaling, 
-00000100: 6c6f 6164 2070 726f 6669 6c65 2c20 7469  load profile, ti
-00000110: 6d65 2073 6572 6965 730d 0a6c 6963 656e  me series..licen
-00000120: 7365 203d 2042 5344 2033 2d43 6c61 7573  se = BSD 3-Claus
-00000130: 6520 4c69 6365 6e73 650d 0a6c 6963 656e  e License..licen
-00000140: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
-00000150: 5345 0d0a 706c 6174 666f 726d 7320 3d20  SE..platforms = 
-00000160: 756e 6978 2c20 6c69 6e75 782c 206f 7378  unix, linux, osx
-00000170: 2c20 7769 6e33 322c 2077 696e 3634 0d0a  , win32, win64..
-00000180: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000190: 742e 6668 2d61 6163 6865 6e2e 6465 2f74  t.fh-aachen.de/t
-000001a0: 6235 3135 3265 2f74 7373 6d0d 0a63 6c61  b5152e/tssm..cla
-000001b0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-000001c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001e0: 332e 3130 0d0a 0950 726f 6772 616d 6d69  3.10...Programmi
-000001f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000200: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000210: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000220: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000230: 2033 2e39 0d0a 0944 6576 656c 6f70 6d65   3.9...Developme
-00000240: 6e74 2053 7461 7475 7320 3a3a 2033 202d  nt Status :: 3 -
-00000250: 2041 6c70 6861 0d0a 094c 6963 656e 7365   Alpha...License
-00000260: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000270: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
-00000280: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
-00000290: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-000002a0: 6573 6561 7263 680d 0a09 4e61 7475 7261  esearch...Natura
-000002b0: 6c20 4c61 6e67 7561 6765 203a 3a20 456e  l Language :: En
-000002c0: 676c 6973 680d 0a09 546f 7069 6320 3a3a  glish...Topic ::
-000002d0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-000002e0: 6e65 6572 696e 6720 3a3a 204d 6174 6865  neering :: Mathe
-000002f0: 6d61 7469 6373 0d0a 0954 6f70 6963 203a  matics...Topic :
-00000300: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000310: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-00000320: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
-00000330: 6475 6c65 730d 0a0d 0a5b 6f70 7469 6f6e  dules....[option
-00000340: 735d 0d0a 7061 636b 6167 6573 203d 2074  s]..packages = t
-00000350: 7373 6d0d 0a69 6e63 6c75 6465 5f70 6163  ssm..include_pac
-00000360: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000370: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000380: 6573 203d 200d 0a09 7365 7475 7074 6f6f  es = ...setuptoo
-00000390: 6c73 3e3d 3632 0d0a 7079 7468 6f6e 5f72  ls>=62..python_r
-000003a0: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
-000003b0: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
-000003c0: 650d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  e....[options.ex
-000003d0: 7472 6173 5f72 6571 7569 7265 5d0d 0a74  tras_require]..t
-000003e0: 6573 7469 6e67 203d 200d 0a09 666c 616b  esting = ...flak
-000003f0: 6538 3e3d 342e 302e 0d0a 0974 6f78 3e3d  e8>=4.0....tox>=
-00000400: 332e 3235 0d0a 0970 7974 6573 743e 3d37  3.25...pytest>=7
-00000410: 2e30 0d0a 0970 7974 6573 742d 636f 763e  .0...pytest-cov>
-00000420: 3d33 2e30 2e30 0d0a 096d 7970 793e 3d30  =3.0.0...mypy>=0
-00000430: 2e39 3631 0d0a 0970 796c 696e 743e 3d32  .961...pylint>=2
-00000440: 2e31 342e 350d 0a09 6973 6f72 743e 3d35  .14.5...isort>=5
-00000450: 2e31 302e 310d 0a09 626c 6163 6b3e 3d32  .10.1...black>=2
-00000460: 322e 362e 300d 0a0d 0a5b 6f70 7469 6f6e  2.6.0....[option
-00000470: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-00000480: 0a63 616c 6375 6c61 7469 6f6e 203d 2070  .calculation = p
-00000490: 792e 7479 7065 640d 0a0d 0a5b 666c 616b  y.typed....[flak
-000004a0: 6538 5d0d 0a6d 6178 2d6c 696e 652d 6c65  e8]..max-line-le
-000004b0: 6e67 7468 203d 2031 3630 0d0a 6578 636c  ngth = 160..excl
-000004c0: 7564 6520 3d20 5f5f 696e 6974 5f5f 2e70  ude = __init__.p
-000004d0: 790d 0a0d 0a5b 7079 6c69 6e74 5d0d 0a6d  y....[pylint]..m
-000004e0: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-000004f0: 2031 3630 0d0a 6469 7361 626c 6520 3d20   160..disable = 
-00000500: 5230 3930 320d 0a0d 0a5b 6567 675f 696e  R0902....[egg_in
-00000510: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000520: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000530: 0a0d 0a                                  ...
+00000020: 203d 2030 2e30 2e34 0d0a 6175 7468 6f72   = 0.0.4..author
+00000030: 203d 2054 6f62 6961 7320 426c 616e 6b65   = Tobias Blanke
+00000040: 2026 2044 6f6d 696e 696b 2046 6973 6368   & Dominik Fisch
+00000050: 6572 0d0a 6465 7363 7269 7074 696f 6e20  er..description 
+00000060: 3d20 5061 636b 6167 6520 746f 2063 7265  = Package to cre
+00000070: 6174 6520 6f75 7420 6f66 2061 2073 696e  ate out of a sin
+00000080: 676c 6520 6c6f 6164 2070 726f 6669 6c65  gle load profile
+00000090: 2061 2070 726f 6669 6c65 2066 6f72 2061   a profile for a
+000000a0: 2077 686f 6c65 2064 6973 7472 6963 7420   whole district 
+000000b0: 7573 696e 6720 7468 6520 6469 7665 7273  using the divers
+000000c0: 6974 7920 6661 6374 6f72 0d0a 6b65 7977  ity factor..keyw
+000000d0: 6f72 6473 203d 206c 6f61 642c 2073 696d  ords = load, sim
+000000e0: 756c 7461 6e65 6974 7920 6661 6374 6f72  ultaneity factor
+000000f0: 2c20 7363 616c 696e 672c 206c 6f61 6420  , scaling, load 
+00000100: 7072 6f66 696c 652c 2074 696d 6520 7365  profile, time se
+00000110: 7269 6573 0d0a 6c69 6365 6e73 6520 3d20  ries..license = 
+00000120: 4253 4420 332d 436c 6175 7365 204c 6963  BSD 3-Clause Lic
+00000130: 656e 7365 0d0a 6c69 6365 6e73 655f 6669  ense..license_fi
+00000140: 6c65 7320 3d20 4c49 4345 4e53 450d 0a70  les = LICENSE..p
+00000150: 6c61 7466 6f72 6d73 203d 2075 6e69 782c  latforms = unix,
+00000160: 206c 696e 7578 2c20 6f73 782c 2077 696e   linux, osx, win
+00000170: 3332 2c20 7769 6e36 340d 0a75 726c 203d  32, win64..url =
+00000180: 2068 7474 7073 3a2f 2f67 6974 2e66 682d   https://git.fh-
+00000190: 6161 6368 656e 2e64 652f 7462 3531 3532  aachen.de/tb5152
+000001a0: 652f 7473 736d 0d0a 636c 6173 7369 6669  e/tssm..classifi
+000001b0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+000001c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001d0: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
+000001e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000200: 203a 3a20 332e 380d 0a09 5072 6f67 7261   :: 3.8...Progra
+00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000220: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000230: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+00000240: 6174 7573 203a 3a20 3320 2d20 416c 7068  atus :: 3 - Alph
+00000250: 610d 0a09 4c69 6365 6e73 6520 3a3a 204f  a...License :: O
+00000260: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
+00000270: 5344 204c 6963 656e 7365 0d0a 0949 6e74  SD License...Int
+00000280: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000290: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
+000002a0: 6368 0d0a 094e 6174 7572 616c 204c 616e  ch...Natural Lan
+000002b0: 6775 6167 6520 3a3a 2045 6e67 6c69 7368  guage :: English
+000002c0: 0d0a 0954 6f70 6963 203a 3a20 5363 6965  ...Topic :: Scie
+000002d0: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
+000002e0: 6e67 203a 3a20 4d61 7468 656d 6174 6963  ng :: Mathematic
+000002f0: 730d 0a09 546f 7069 6320 3a3a 2053 6f66  s...Topic :: Sof
+00000300: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+00000310: 7420 3a3a 204c 6962 7261 7269 6573 203a  t :: Libraries :
+00000320: 3a20 5079 7468 6f6e 204d 6f64 756c 6573  : Python Modules
+00000330: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000340: 6163 6b61 6765 7320 3d20 7473 736d 0d0a  ackages = tssm..
+00000350: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000360: 6461 7461 203d 2054 7275 650d 0a69 6e73  data = True..ins
+00000370: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000380: 0d0a 0973 6574 7570 746f 6f6c 733e 3d36  ...setuptools>=6
+00000390: 320d 0a70 7974 686f 6e5f 7265 7175 6972  2..python_requir
+000003a0: 6573 203d 203e 3d33 2e38 0d0a 7a69 705f  es = >=3.8..zip_
+000003b0: 7361 6665 203d 2046 616c 7365 0d0a 0d0a  safe = False....
+000003c0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+000003d0: 7265 7175 6972 655d 0d0a 7465 7374 696e  require]..testin
+000003e0: 6720 3d20 0d0a 0966 6c61 6b65 383e 3d34  g = ...flake8>=4
+000003f0: 2e30 2e31 0d0a 0974 6f78 3e3d 332e 3235  .0.1...tox>=3.25
+00000400: 0d0a 0970 7974 6573 743e 3d37 2e30 0d0a  ...pytest>=7.0..
+00000410: 0970 7974 6573 742d 636f 763e 3d33 2e30  .pytest-cov>=3.0
+00000420: 2e30 0d0a 096d 7970 793e 3d30 2e39 3631  .0...mypy>=0.961
+00000430: 0d0a 0970 796c 696e 743e 3d32 2e31 342e  ...pylint>=2.14.
+00000440: 350d 0a09 6973 6f72 743e 3d35 2e31 302e  5...isort>=5.10.
+00000450: 310d 0a09 626c 6163 6b3e 3d32 322e 362e  1...black>=22.6.
+00000460: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  0....[options.pa
+00000470: 636b 6167 655f 6461 7461 5d0d 0a63 616c  ckage_data]..cal
+00000480: 6375 6c61 7469 6f6e 203d 2070 792e 7479  culation = py.ty
+00000490: 7065 640d 0a0d 0a5b 666c 616b 6538 5d0d  ped....[flake8].
+000004a0: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
+000004b0: 203d 2031 3630 0d0a 6578 636c 7564 6520   = 160..exclude 
+000004c0: 3d20 5f5f 696e 6974 5f5f 2e70 790d 0a65  = __init__.py..e
+000004d0: 7874 656e 642d 6967 6e6f 7265 203d 2045  xtend-ignore = E
+000004e0: 3230 330d 0a0d 0a5b 7079 6c69 6e74 5d0d  203....[pylint].
+000004f0: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
+00000500: 203d 2031 3630 0d0a 6469 7361 626c 6520   = 160..disable 
+00000510: 3d20 5230 3930 320d 0a0d 0a5b 6567 675f  = R0902....[egg_
+00000520: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000530: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000540: 300d 0a0d 0a                             0....
```

### Comparing `tssm-0.0.2rc1/setup.py` & `tssm-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tssm-0.0.2rc1/tssm/value_storage.py` & `tssm-0.0.4/tssm/value_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,65 @@
 """
 python script for the value storage dataclass and its functions
 """
-
+from __future__ import annotations
 
 from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
-from numpy.typing import NDArray  # type: ignore
-from pandas import read_csv as pd_read_csv
+
+from tssm.utils.dict_casting import from_dict, to_dict
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from numpy.typing import NDArray
+
+
+class NoColumnError(KeyError):
+    """Error raised if column is not in dataframe"""
+
+    def __init__(self, key: str):
+        super().__init__(f"no such column {key} in pandas Dataframe")
+
+
+class NoDataFrameError(FileNotFoundError):
+    """Error if dataframe can not be located"""
+
+    def __init__(self, path: str):
+        super().__init__(f"pandas Dataframe not found: {path}")
 
 
 @dataclass
-class ValueStorage:
+class DataStorage:
     """class to store the original, new, average, scaling and date values"""
 
-    average: NDArray[np.float64] = field(default_factory=lambda: np.zeros(0))
+    reference: NDArray[np.float64] = field(default_factory=lambda: np.zeros(0))
     original: NDArray[np.float64] = field(default_factory=lambda: np.zeros(0))
     scaling: NDArray[np.float64] = field(default_factory=lambda: np.zeros(0))
     new: NDArray[np.float64] = field(default_factory=lambda: np.zeros(0))
-    date: NDArray[np.float64] = field(default_factory=lambda: np.zeros(0))
+    _date: NDArray[np.float64] = field(default_factory=lambda: np.zeros(0))
+    time_step: NDArray[np.float64] | float | None = None
+
+    def _get_date(self) -> NDArray[np.float64]:
+        """
+        get date
+        """
+        return self._date
+
+    def _set_date(self, value: NDArray[np.float64]):
+        """
+        set date and determine time step
+        """
+        self._date = value
+        self._determine_time_step()
+
+    date = property(fget=_get_date, fset=_set_date, doc="date of original time series")
 
     def read_profile_from_csv_with_date(
         self,
         path: str,
         column_of_load: str,
         column_of_date: str,
         *,
@@ -107,120 +143,132 @@
         """
         set load profile from numpy array
         :param load_profile: load profile as numpy array
         """
         self.original = load_profile
 
     @staticmethod
-    def _read_dataframe_from_csv(path: str, separator: str = ",", decimal: str = ".") -> pd.DataFrame:
+    def _read_dataframe_from_csv(path: str | Path, separator: str = ",", decimal: str = ".") -> pd.DataFrame:
         """
         read dataframe from csv file\n
         :param path: path of csv file from which the dataframe should be read
         :param separator: seperator sign between csv columns (default is ,)
         :param decimal: decimal sign in csv file (default is .)
         """
         # try to read csv file if not found raise an exception
         try:
-            data_frame: pd.DataFrame = pd_read_csv(path, sep=separator, decimal=decimal)
+            data_frame: pd.DataFrame = pd.read_csv(path, sep=separator, decimal=decimal)
         except FileNotFoundError as exception:
-            raise FileNotFoundError(f"pandas Dataframe not found: {path}") from exception
+            raise NoDataFrameError(f"{path}") from exception
         return data_frame
 
     @staticmethod
     def _get_date_from_dataframe(data_frame: pd.DataFrame, column_of_date: str) -> pd.Series:
         """
         get date from pandas Dataframe and check if column exists\n
         :param data_frame: pandas DataFrame to read the date from
         :param column_of_date: column name of date in Dataframe
         :return: pandas series of date
         """
         # try to get date from column otherwise raise column not found error
         try:
             date = data_frame[column_of_date]
         except KeyError as exception:
-            raise KeyError("no such Date column in pandas Dataframe") from exception
+            raise NoColumnError(column_of_date) from exception
         return date
 
     def _get_profile_from_dataframe(self, data_frame: pd.DataFrame, column_of_load: str) -> None:
         """
         get profile from pandas Dataframe and check if column exists\n
         :param data_frame: pandas DataFrame to read the profile from
         :param column_of_load: column name of profile in Dataframe
         :return: pandas series of profile
         """
         # try to get load profile from column otherwise raise column not found error
         try:
             self.original = data_frame[column_of_load].to_numpy(dtype=np.float64)
         except KeyError as exception:
-            raise KeyError("no such column in pandas Dataframe to read values from") from exception
+            raise NoColumnError(column_of_load) from exception
 
     def _reformat_date(self, date: pd.Series, *, date_format: str = "%Y-%m-%d %H:%M:%S") -> None:
         """
         reformat date input as pandas Dataframe to a numpy array\n
         :param date: pandas series including the date
         :param date_format: date time format if necessary (default YYYY-MM-DD hh:mm:ss)
         Link for date format https://docs.python.org/3/library/datetime.html#strftime-and-strptime-behavior
         """
         date = pd.to_datetime(date, format=date_format)
         self.date = date.to_numpy(dtype="datetime64[s]")
 
-    def scale_scaling_profile_2_same_sum(self) -> None:
-        """
-        scales the scaling profile to the same sum of the original load
-        """
-        self.scaling = self.scaling / self.scaling.sum() * self.original.sum()
-
-    def set_scaling_profile_from_numpy_array(self, load_profile: NDArray[np.float64], *, same_sum: bool = False) -> None:
+    def set_scaling_profile_from_numpy_array(self, load_profile: NDArray[np.float64]) -> None:
         """
         set scaling profile from numpy array
         :param load_profile: load profile as numpy array
-        :param same_sum: size scaling profile to the same sum as the original profile (default=False)
         """
         # set scaling profile
         self.scaling = load_profile
-        # calculate same sum if wanted
-        if same_sum:
-            self.scale_scaling_profile_2_same_sum()
 
-    def set_scaling_profile_from_pandas_series(self, load_profile: pd.Series, *, same_sum: bool = False) -> None:
+    def set_scaling_profile_from_pandas_series(self, load_profile: pd.Series) -> None:
         """
         set scaling profile from pandas series
         :param load_profile: load profile as pandas series
-        :param same_sum: size scaling profile to the same sum as the original profile (default=False)
         """
         # set scaling profile
         self.scaling = load_profile.to_numpy(dtype=np.float64)
-        # calculate same sum if wanted
-        if same_sum:
-            self.scale_scaling_profile_2_same_sum()
 
-    def read_scaling_profile_from_dataframe(self, data_frame: pd.DataFrame, column_of_scaled_profile: str, *, same_sum: bool = False) -> None:
+    def read_scaling_profile_from_dataframe(self, data_frame: pd.DataFrame, column_of_scaled_profile: str) -> None:
         """
         read scaling profile from pandas dataframe
         :param data_frame: pandas dataframe to read profile from
         :param column_of_scaled_profile: column name of scaling profile in pandas dataframe
-        :param same_sum: size scaling profile to the same sum as the original profile (default=False)
         """
         # set scaling profile
         self.scaling = data_frame[column_of_scaled_profile].to_numpy(dtype=np.float64)
-        # calculate same sum if wanted
-        if same_sum:
-            self.scale_scaling_profile_2_same_sum()
 
-    def read_scaling_profile_from_csv(
-        self, path: str, column_of_scaled_profile: str, *, separator: str = ",", decimal: str = ".", same_sum: bool = False
-    ) -> None:
+    def read_scaling_profile_from_csv(self, path: str, column_of_scaled_profile: str, *, separator: str = ",", decimal: str = ".") -> None:
         """
         read profile to be scaled from csv file\n
         :param path: path of csv file from which the dataframe should be read
         :param column_of_scaled_profile: column name of scaling profile in csv
         :param separator: seperator sign between csv columns (default is ,)
         :param decimal: decimal sign in csv file (default is .)
-        :param same_sum: size scaling profile to the same sum as the original profile (default=False)
         """
         # get pandas dataframe from csv file
         data_frame = self._read_dataframe_from_csv(path, separator, decimal)
         # set scaling profile
         self.scaling = data_frame[column_of_scaled_profile].to_numpy(dtype=np.float64)
-        # calculate same sum if wanted
-        if same_sum:
-            self.scale_scaling_profile_2_same_sum()
+
+    def _determine_time_step(self) -> None:
+        """
+        determine the time step of the date array
+        """
+        # if the length of the date is longer then one determine the time step
+        if len(self.date) > 1:
+            # determine the time step as an array
+            time_step = np.array(np.diff(self.date), dtype=np.float64)
+            # if all time steps are the same return the time step as a float
+            if np.allclose(time_step, time_step[0]):
+                self.time_step = time_step[0] / 3600
+                return
+            # otherwise append the first entry at the end and return the array
+            self.time_step = np.append(time_step, time_step[0]) / 3600
+            return
+
+    def delete_zero_values(self) -> None:
+        """
+        delete the values in the data where the timestep is zero\n
+        """
+        # check if time step is an array (so different for every timestep)
+        if isinstance(self.time_step, np.ndarray):
+            # delete values in the original data
+            self.original = np.delete(self.original, np.isclose(self.time_step, 0))
+            # delete values in the date data
+            self._date = np.delete(self._date, np.isclose(self.time_step, 0))
+            # delete zero entries in the time step array
+            self.time_step = np.delete(self.time_step, np.isclose(self.time_step, 0))
+
+    def to_dict(self) -> dict:
+        return to_dict(self)
+
+    def from_dict(self, dictionary: dict) -> None:
+        from_dict(self, dictionary)
+        self.date = self.date.astype("datetime64[s]")
```

### Comparing `tssm-0.0.2rc1/tssm.egg-info/PKG-INFO` & `tssm-0.0.4/tssm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tssm
-Version: 0.0.2rc1
+Version: 0.0.4
 Summary: Package to create out of a single load profile a profile for a whole district using the diversity factor
 Home-page: https://git.fh-aachen.de/tb5152e/tssm
 Author: Tobias Blanke & Dominik Fischer
 License: BSD 3-Clause License
 Keywords: load,simultaneity factor,scaling,load profile,time series
 Platform: unix
 Platform: linux
@@ -26,74 +26,77 @@
 License-File: LICENSE
 
 [![Status](https://img.shields.io/pypi/status/tssm)](https://pypi.python.org/pypi/tssm)
 [![Version](https://img.shields.io/pypi/v/tssm.svg)](https://pypi.python.org/pypi/tssm)
 [![Python Version](https://img.shields.io/pypi/pyversions/tssm)](https://pypi.python.org/pypi/tssm)
 [![Wheel](https://img.shields.io/pypi/wheel/tssm)](https://pypi.python.org/pypi/tssm)
 [![PyPI - License](https://img.shields.io/pypi/l/tssm)](https://opensource.org/licenses/BSD-3-Clause)
+
+[![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases)
+[![OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/issues)
+
 [![Documentation Status](https://readthedocs.org/projects/tssm/badge/?version=latest)](https://tssm.readthedocs.io/en/latest/?badge=latest)
-[![coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
 [![pipeline status](https://git.fh-aachen.de/tb5152e/tssm/badges/main/pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases)
-[![Pylint](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/pylint.svg?job=pylint)](https://pylint.pycqa.org/en/latest/)
+[![coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
+[![Pylint](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/pylint.svg&job=pylint)](https://pylint.pycqa.org/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](http://mypy-lang.org/)
 [![security: bandit](https://img.shields.io/badge/security-bandit-success.svg)](https://github.com/PyCQA/bandit)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main)
-[![OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/issues)
 
 
-<a href="https://www.fh-aachen.de/forschung/solar-institut-juelich"><img src="https://www.fh-aachen.de/fileadmin/ins/ins_sij/Wortmarke_SIJ_ts_web.jpg" alt="Forschungszentrum Juelich Logo"></a> 
+<a href="https://www.fh-aachen.de/forschung/solar-institut-juelich"><img src="https://www.fh-aachen.de/fileadmin/ins/ins_sij/Wortmarke_SIJ_ts_web.jpg" 
+alt="Solar Institute Juelich Logo"></a> 
 
 # Time Series Scaling Module  (TSSM)
-TSSM is a python package for the scaling of time series. 
+<img src="./docs/sources/_static/Logo.svg" width="100" align="left">
+
+**TSSM** is a python package for the up-scaling of time series or load such as electricity, heating, etc. 
+
 
 **Warning**
 ```{warning} 
 This package is under heavy development!
 ```
 
 ## Getting started
-### Install tssm
-Install tssm directly from PyPi as follows. It is recommended to set up a fresh Conda environment before using this package by following these steps:
 
-* Install Miniconda or update your conda installation with `conda update conda`
-* Create a new environment with `conda create -n <environmentName> python=<pythonVersion>`. The python version to be specified should be greater than python 3.8. 
-* Activate the environment with `source activate <environmentName>` on Linux/MacOS or `activate <environmentName>` on Windows
-* Clone tssm with `git clone https://git.fh-aachen.de/tb5152e/tssm.git`
-* Install tssm with `pip install -e <path_to_tssm_package>`
-* Verify your tssm package installtion by running the configured automated tests. Go to your tssm top-level directory and type `pytest`
+### Install TSSM
+
+Install tssm directly from PyPi as follows: 
 
-Or you can also directly install tssm package from PyPi with the following command
 ```console
 pip install tssm
 ```
 
+Further installation instructions can be found in the [**documentation**](http://tssm.rtfd.io/) under 'Getting started'.
+
+
 ### Usage
 
 example usages can be found in the [**examples'**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples) folder.
 
 
 #### Basic workflow
 
 A small example how tssm can be used is described as follows:
 
 ```python
-# import module
-from tssm import TimeSeriesScalingModule as tssm
+# import module and Daily period variable
+from tssm import TimeSeriesScalingModule as tssm, DAILY
 
 # initialize class with a number of buildings of 202 with a simultaneity factor of 0.786
-df_test = tssm(number_of_buildings=202, simultaneity_factor=0.786)
+scaling = tssm(number_of_buildings=202, simultaneity_factor=0.786)
 # read profile from data.csv file and use the Electricity and Date column
-df_test.values.read_profile_from_csv_with_date(path="./data.csv", column_of_load="Electricity", column_of_date="Date")
-# calculate linear scaled values with a daily (period=1) simultaneity factor and average value
-daily_scaled_values = df_test.calculate_linear(period=1)
+scaling.data.read_profile_from_csv_with_date(path="./data.csv", column_of_load="Electricity", column_of_date="Date")
+# calculate linear scaled values with a daily simultaneity factor and average value
+daily_scaled_values = scaling.calculate_using_average_values(period=DAILY)
 ```
 
 #### Examples
 A [**first example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/example_linear.py) shows the linear approach. It scales the time series between the scaled time series and an average.
 
 A [**second example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/example_scaling.py) shows the scaling approach. It scales the time series between the scaled time series and a scaling time 
 series.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tssm Version: 0.0.2rc1 Summary: Package to create
-out of a single load profile a profile for a whole district using the diversity
+Metadata-Version: 2.1 Name: tssm Version: 0.0.4 Summary: Package to create out
+of a single load profile a profile for a whole district using the diversity
 factor Home-page: https://git.fh-aachen.de/tb5152e/tssm Author: Tobias Blanke &
 Dominik Fischer License: BSD 3-Clause License Keywords: load,simultaneity
 factor,scaling,load profile,time series Platform: unix Platform: linux
 Platform: osx Platform: win32 Platform: win64 Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Development Status :: 3 -
 Alpha Classifier: License :: OSI Approved :: BSD License Classifier: Intended
@@ -13,74 +13,67 @@
 Description-Content-Type: text/markdown Provides-Extra: testing License-File:
 LICENSE [![Status](https://img.shields.io/pypi/status/tssm)](https://
 pypi.python.org/pypi/tssm) [![Version](https://img.shields.io/pypi/v/tssm.svg)]
 (https://pypi.python.org/pypi/tssm) [![Python Version](https://img.shields.io/
 pypi/pyversions/tssm)](https://pypi.python.org/pypi/tssm) [![Wheel](https://
 img.shields.io/pypi/wheel/tssm)](https://pypi.python.org/pypi/tssm) [![PyPI -
 License](https://img.shields.io/pypi/l/tssm)](https://opensource.org/licenses/
-BSD-3-Clause) [![Documentation Status](https://readthedocs.org/projects/tssm/
+BSD-3-Clause) [![Last Commit](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/
+artifacts/main/raw/public/badges/last_commit.svg?job=badges)](https://git.fh-
+aachen.de/tb5152e/tssm/-/commits/main) [![Last Release](https://git.fh-
+aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/
+last_release.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/
+main) [![Latest Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/
+release.svg)](https://git.fh-aachen.de/tb5152e/diversityfactor/-/releases) [!
+[OpenIssues](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/
+public/badges/open_issues.svg?job=badges)](https://git.fh-aachen.de/tb5152e/
+tssm/-/issues) [![Documentation Status](https://readthedocs.org/projects/tssm/
 badge/?version=latest)](https://tssm.readthedocs.io/en/latest/?badge=latest) [!
-[coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
-coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [!
 [pipeline status](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
-pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [![Latest
-Release](https://git.fh-aachen.de/tb5152e/tssm/-/badges/release.svg)](https://
-git.fh-aachen.de/tb5152e/diversityfactor/-/releases) [![Pylint](https://git.fh-
-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/
-pylint.svg?job=pylint)](https://pylint.pycqa.org/en/latest/) [![Code style:
+pipeline.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [!
+[coverage report](https://git.fh-aachen.de/tb5152e/tssm/badges/main/
+coverage.svg)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/main) [![Pylint]
+(https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/main/raw/public/pylint/
+pylint.svg&job=pylint)](https://pylint.pycqa.org/en/latest/) [![Code style:
 black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/
-%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
-pycqa.github.io/isort/) [![Checked with mypy](http://www.mypy-lang.org/static/
-mypy_badge.svg)](http://mypy-lang.org/) [![security: bandit](https://
-img.shields.io/badge/security-bandit-success.svg)](https://github.com/PyCQA/
-bandit) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-
-1f425f.svg)](https://www.python.org/) [![Last Commit](https://git.fh-aachen.de/
-tb5152e/tssm/-/jobs/artifacts/main/raw/public/badges/
-last_commit.svg?job=badges)](https://git.fh-aachen.de/tb5152e/tssm/-/commits/
-main) [![Last Release](https://git.fh-aachen.de/tb5152e/tssm/-/jobs/artifacts/
-main/raw/public/badges/last_release.svg?job=badges)](https://git.fh-aachen.de/
-tb5152e/tssm/-/commits/main) [![OpenIssues](https://git.fh-aachen.de/tb5152e/
-tssm/-/jobs/artifacts/main/raw/public/badges/open_issues.svg?job=badges)]
-(https://git.fh-aachen.de/tb5152e/tssm/-/issues) [Forschungszentrum_Juelich
-Logo] # Time Series Scaling Module (TSSM) TSSM is a python package for the
-scaling of time series. **Warning** ```{warning} This package is under heavy
-development! ``` ## Getting started ### Install tssm Install tssm directly from
-PyPi as follows. It is recommended to set up a fresh Conda environment before
-using this package by following these steps: * Install Miniconda or update your
-conda installation with `conda update conda` * Create a new environment with
-`conda create -n  python=`. The python version to be specified should be
-greater than python 3.8. * Activate the environment with `source activate ` on
-Linux/MacOS or `activate ` on Windows * Clone tssm with `git clone https://
-git.fh-aachen.de/tb5152e/tssm.git` * Install tssm with `pip install -e ` *
-Verify your tssm package installtion by running the configured automated tests.
-Go to your tssm top-level directory and type `pytest` Or you can also directly
-install tssm package from PyPi with the following command ```console pip
-install tssm ``` ### Usage example usages can be found in the [**examples'**]
-(https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples) folder. #### Basic
-workflow A small example how tssm can be used is described as follows:
-```python # import module from tssm import TimeSeriesScalingModule as tssm #
-initialize class with a number of buildings of 202 with a simultaneity factor
-of 0.786 df_test = tssm(number_of_buildings=202, simultaneity_factor=0.786) #
-read profile from data.csv file and use the Electricity and Date column
-df_test.values.read_profile_from_csv_with_date(path="./data.csv",
-column_of_load="Electricity", column_of_date="Date") # calculate linear scaled
-values with a daily (period=1) simultaneity factor and average value
-daily_scaled_values = df_test.calculate_linear(period=1) ``` #### Examples A
-[**first example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/
-example_linear.py) shows the linear approach. It scales the time series between
-the scaled time series and an average. A [**second example**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/examples/example_scaling.py) shows the
-scaling approach. It scales the time series between the scaled time series and
-a scaling time series. A [**third example**](https://git.fh-aachen.de/tb5152e/
-tssm/-/blob/main/examples/example_normal_distribution.py) shows the normal
-distribution approach. It scales the time series by applying a normal
-distribution to every time step. A [**fourth example**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/examples/
-example_of_different_method_2_import_profiles.py) shows the different ways to
-import the data. A [**fifth example**](https://git.fh-aachen.de/tb5152e/tssm/-/
-blob/main/examples/example_speed_comparison.py) shows the speed of the
-different approaches. ### License The module is licensed under BSD 3-Clause
-License. Further, License information can be found [**here**](https://git.fh-
-aachen.de/tb5152e/tssm/-/blob/main/LICENSE). ### Reference ### Acknowledgements
-## Content The documentation of the tssm code can be found [**here**](http://
-tssm.rtfd.io/).
+%20imports-isort-%231674b1&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](http://
+mypy-lang.org/) [![security: bandit](https://img.shields.io/badge/security-
+bandit-success.svg)](https://github.com/PyCQA/bandit) [![made-with-python]
+(https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://
+www.python.org/) [Solar_Institute_Juelich_Logo] # Time Series Scaling Module
+(TSSM) [./docs/sources/_static/Logo.svg] **TSSM** is a python package for the
+up-scaling of time series or load such as electricity, heating, etc.
+**Warning** ```{warning} This package is under heavy development! ``` ##
+Getting started ### Install TSSM Install tssm directly from PyPi as follows:
+```console pip install tssm ``` Further installation instructions can be found
+in the [**documentation**](http://tssm.rtfd.io/) under 'Getting started'. ###
+Usage example usages can be found in the [**examples'**](https://git.fh-
+aachen.de/tb5152e/tssm/-/blob/main/examples) folder. #### Basic workflow A
+small example how tssm can be used is described as follows: ```python # import
+module and Daily period variable from tssm import TimeSeriesScalingModule as
+tssm, DAILY # initialize class with a number of buildings of 202 with a
+simultaneity factor of 0.786 scaling = tssm(number_of_buildings=202,
+simultaneity_factor=0.786) # read profile from data.csv file and use the
+Electricity and Date column scaling.data.read_profile_from_csv_with_date
+(path="./data.csv", column_of_load="Electricity", column_of_date="Date") #
+calculate linear scaled values with a daily simultaneity factor and average
+value daily_scaled_values = scaling.calculate_using_average_values
+(period=DAILY) ``` #### Examples A [**first example**](https://git.fh-
+aachen.de/tb5152e/tssm/-/blob/main/examples/example_linear.py) shows the linear
+approach. It scales the time series between the scaled time series and an
+average. A [**second example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/
+main/examples/example_scaling.py) shows the scaling approach. It scales the
+time series between the scaled time series and a scaling time series. A
+[**third example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/examples/
+example_normal_distribution.py) shows the normal distribution approach. It
+scales the time series by applying a normal distribution to every time step. A
+[**fourth example**](https://git.fh-aachen.de/tb5152e/tssm/-/blob/main/
+examples/example_of_different_method_2_import_profiles.py) shows the different
+ways to import the data. A [**fifth example**](https://git.fh-aachen.de/
+tb5152e/tssm/-/blob/main/examples/example_speed_comparison.py) shows the speed
+of the different approaches. ### License The module is licensed under BSD 3-
+Clause License. Further, License information can be found [**here**](https://
+git.fh-aachen.de/tb5152e/tssm/-/blob/main/LICENSE). ### Reference ###
+Acknowledgements ## Content The documentation of the tssm code can be found
+[**here**](http://tssm.rtfd.io/).
```

