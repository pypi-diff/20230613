# Comparing `tmp/ansys_optislang_core-0.2.1.tar.gz` & `tmp/ansys_optislang_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_optislang_core-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_optislang_core-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_optislang_core-0.2.1.tar` & `ansys_optislang_core-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1089 2023-05-16 13:46:29.322744 ansys_optislang_core-0.2.1/LICENSE
--rw-r--r--   0        0        0     7402 2023-05-16 13:46:29.322744 ansys_optislang_core-0.2.1/README.rst
--rw-r--r--   0        0        0     2262 2023-05-16 13:46:29.326744 ansys_optislang_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-05-16 13:46:29.326744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/__init__.py
--rw-r--r--   0        0        0     2174 2023-05-16 13:46:29.326744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/encoding.py
--rw-r--r--   0        0        0      946 2023-05-16 13:46:29.326744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/errors.py
--rw-r--r--   0        0        0     2250 2023-05-16 13:46:29.326744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp
--rw-r--r--   0        0        0   235264 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb
--rw-r--r--   0        0        0     2659 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py
--rw-r--r--   0        0        0    28174 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf
--rw-r--r--   0        0        0    70667 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf
--rw-r--r--   0        0        0    18887 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf
--rw-r--r--   0        0        0    47797 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf
--rw-r--r--   0        0        0   212239 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf
--rw-r--r--   0        0        0      299 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.bat
--rw-r--r--   0        0        0     1812 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py
--rw-r--r--   0        0        0     4438 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s
--rw-r--r--   0        0        0      194 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.sh
--rw-r--r--   0        0        0     1401 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt
--rw-r--r--   0        0        0     1989 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt
--rw-r--r--   0        0        0     3442 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py
--rw-r--r--   0        0        0     2927 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py
--rw-r--r--   0        0        0     4329 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py
--rw-r--r--   0        0        0     3848 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py
--rw-r--r--   0        0        0     3274 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py
--rw-r--r--   0        0        0     3838 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py
--rw-r--r--   0        0        0     9630 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py
--rw-r--r--   0        0        0     6171 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py
--rw-r--r--   0        0        0      475 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py
--rw-r--r--   0        0        0     2601 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py
--rw-r--r--   0        0        0     1251 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py
--rw-r--r--   0        0        0      752 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py
--rw-r--r--   0        0        0     1367 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py
--rw-r--r--   0        0        0      626 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py
--rw-r--r--   0        0        0     4089 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py
--rw-r--r--   0        0        0     2872 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac
--rw-r--r--   0        0        0      686 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out
--rw-r--r--   0        0        0    10909 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s
--rw-r--r--   0        0        0      686 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out
--rw-r--r--   0        0        0    10785 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s
--rw-r--r--   0        0        0    34914 2023-05-16 13:46:29.330744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz
--rw-r--r--   0        0        0     2068 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py
--rw-r--r--   0        0        0     5289 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py
--rw-r--r--   0        0        0     1010 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py
--rw-r--r--   0        0        0     4543 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py
--rw-r--r--   0        0        0       86 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/__init__.py
--rw-r--r--   0        0        0     1770 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/downloads.py
--rw-r--r--   0        0        0     5759 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/examples.py
--rw-r--r--   0        0        0     8841 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/logging.py
--rw-r--r--   0        0        0    32226 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/nodes.py
--rw-r--r--   0        0        0    24773 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/optislang.py
--rw-r--r--   0        0        0    28540 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/osl_process.py
--rw-r--r--   0        0        0    28603 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/osl_server.py
--rw-r--r--   0        0        0     7045 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/project.py
--rw-r--r--   0        0        0   134430 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/project_parametric.py
--rw-r--r--   0        0        0    39038 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/server_commands.py
--rw-r--r--   0        0        0     9224 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/server_queries.py
--rw-r--r--   0        0        0    96655 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/tcp_osl_server.py
--rw-r--r--   0        0        0    13862 2023-05-16 13:46:29.334744 ansys_optislang_core-0.2.1/src/ansys/optislang/core/utils.py
--rw-r--r--   0        0        0     9099 1970-01-01 00:00:00.000000 ansys_optislang_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-13 11:45:27.244387 ansys_optislang_core-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7401 2023-06-13 11:45:27.244387 ansys_optislang_core-0.3.0/README.rst
+-rw-r--r--   0        0        0     2262 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1373 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/__init__.py
+-rw-r--r--   0        0        0     2174 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/encoding.py
+-rw-r--r--   0        0        0      946 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/errors.py
+-rw-r--r--   0        0        0     2250 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp
+-rw-r--r--   0        0        0   235264 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb
+-rw-r--r--   0        0        0     2659 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py
+-rw-r--r--   0        0        0    28174 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf
+-rw-r--r--   0        0        0    70667 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf
+-rw-r--r--   0        0        0    18887 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf
+-rw-r--r--   0        0        0    47797 2023-06-13 11:45:27.252387 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf
+-rw-r--r--   0        0        0   212239 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf
+-rw-r--r--   0        0        0      299 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.bat
+-rw-r--r--   0        0        0     1812 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py
+-rw-r--r--   0        0        0     4438 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s
+-rw-r--r--   0        0        0      194 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.sh
+-rw-r--r--   0        0        0     1401 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt
+-rw-r--r--   0        0        0     1989 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt
+-rw-r--r--   0        0        0     3442 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py
+-rw-r--r--   0        0        0     2927 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py
+-rw-r--r--   0        0        0     4329 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py
+-rw-r--r--   0        0        0     3848 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py
+-rw-r--r--   0        0        0     3274 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py
+-rw-r--r--   0        0        0     3838 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py
+-rw-r--r--   0        0        0     9630 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py
+-rw-r--r--   0        0        0     6171 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py
+-rw-r--r--   0        0        0      475 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py
+-rw-r--r--   0        0        0     2601 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py
+-rw-r--r--   0        0        0     1251 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py
+-rw-r--r--   0        0        0      752 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py
+-rw-r--r--   0        0        0     1367 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py
+-rw-r--r--   0        0        0      626 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py
+-rw-r--r--   0        0        0     4089 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py
+-rw-r--r--   0        0        0     2872 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac
+-rw-r--r--   0        0        0      686 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out
+-rw-r--r--   0        0        0    10909 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s
+-rw-r--r--   0        0        0      686 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out
+-rw-r--r--   0        0        0    10785 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s
+-rw-r--r--   0        0        0    34914 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz
+-rw-r--r--   0        0        0     2068 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py
+-rw-r--r--   0        0        0     5289 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py
+-rw-r--r--   0        0        0     1010 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py
+-rw-r--r--   0        0        0     4543 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py
+-rw-r--r--   0        0        0       86 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/__init__.py
+-rw-r--r--   0        0        0     1770 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/downloads.py
+-rw-r--r--   0        0        0     5759 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/examples.py
+-rw-r--r--   0        0        0     8841 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/logging.py
+-rw-r--r--   0        0        0    32226 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/nodes.py
+-rw-r--r--   0        0        0    30916 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/optislang.py
+-rw-r--r--   0        0        0    40761 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/osl_process.py
+-rw-r--r--   0        0        0    31543 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/osl_server.py
+-rw-r--r--   0        0        0     7045 2023-06-13 11:45:27.256388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/project.py
+-rw-r--r--   0        0        0   145170 2023-06-13 11:45:27.260388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/project_parametric.py
+-rw-r--r--   0        0        0    39173 2023-06-13 11:45:27.260388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/server_commands.py
+-rw-r--r--   0        0        0     9224 2023-06-13 11:45:27.260388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/server_queries.py
+-rw-r--r--   0        0        0   103118 2023-06-13 11:45:27.260388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/tcp_osl_server.py
+-rw-r--r--   0        0        0    14950 2023-06-13 11:45:27.260388 ansys_optislang_core-0.3.0/src/ansys/optislang/core/utils.py
+-rw-r--r--   0        0        0     9098 1970-01-01 00:00:00.000000 ansys_optislang_core-0.3.0/PKG-INFO
```

### Comparing `ansys_optislang_core-0.2.1/LICENSE` & `ansys_optislang_core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/README.rst` & `ansys_optislang_core-0.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 --------
 PyOptiSLang is a Python wrapper for Ansys optiSLang. It supports Pythonic
 access to Ansys optiSLang to be able to communicate with Ansys optiSLang directly from Python.
 The latest ``ansys-optislang`` package provides these capabilities:
 
 - Starting and managing local instances of Ansys optiSLang
 - Remote connections to Ansys optiSLang instances via TCP/IP
-- Create new Ansys optiSLang project	
+- Create new Ansys optiSLang project
 - Open existing Ansys optiSLang project
 - Control Ansys optiSLang project execution
 - Save Ansys optiSLang project
 - Execute classic Ansys optiSLang Python API script on backend side
 - Evaluate designs on root project level
```

### Comparing `ansys_optislang_core-0.2.1/pyproject.toml` & `ansys_optislang_core-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-optislang-core"
-version = "0.2.1"
+version = "0.3.0"
 description = "A Python wrapper for Ansys optiSLang application."
 readme = "README.rst"
 requires-python = ">=3.7,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -34,23 +34,23 @@
     "importlib-metadata>=4.0,<7",
     "psutil>=5.9"
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.3.1",
-    "pytest-cov==4.0.0",
+    "pytest-cov==4.1.0",
     "matplotlib>=3.5.3",
 ]
 doc = [
-    "ansys-sphinx-theme==0.9.8",
+    "ansys-sphinx-theme==0.9.9",
     "matplotlib==3.7.1",
     "numpydoc==1.5.0",
     "pypandoc==1.11",
-    "Sphinx==7.0.0",
+    "Sphinx==7.0.1",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
     "sphinxcontrib-images==0.9.4",
 ]
 build = [
     "build>=0.8.0",
     "twine>=4.0.1",
```

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/__init__.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/encoding.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/encoding.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/errors.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/downloads.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/examples/examples.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/logging.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/nodes.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/optislang.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/optislang.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Contains Optislang class, which provides the Python API for the optiSLang app."""
 from __future__ import annotations
 
 from pathlib import Path
-from typing import TYPE_CHECKING, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Iterable, Mapping, Optional, Sequence, Tuple, Union
 
 from importlib_metadata import version
 
 from ansys.optislang.core import LOG
 from ansys.optislang.core.project import Project
 from ansys.optislang.core.tcp_osl_server import TcpOslServer
 
@@ -44,18 +44,56 @@
         when ``host`` and ``port`` parameters are specified. Here is how
         this parameter is used:
 
         - If the project file exists, it is opened.
         - If the project file does not exist, a project is created in the specified path.
         - If the path is ``None``, a new project is created in the temporary directory.
 
+    batch : bool, optional
+        Determines whether to start optiSLang server in batch mode. Defaults to ``True``.
+    port_range : Tuple[int, int], optional
+        Defines the port range for optiSLang server. Defaults to ``None``.
+    no_run : bool, optional
+        Determines whether not to run the specified project when started in batch mode.
+        Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
     no_save : bool, optional
         Whether to save the specified project after all other actions are completed.
         The default is ``False``. This parameter is ignored when ``host`` and
         ``port`` parameters are specified.
+
+        .. note:: Only supported in batch mode.
+
+    force : bool, optional
+        Determines whether to force opening/processing specified project when started in batch mode
+        even if issues occur.
+        Defaults to ``True``.
+
+        .. note:: Only supported in batch mode.
+
+    reset : bool, optional
+        Determines whether to reset specified project after load.
+        Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    auto_relocate : bool, optional
+        Determines whether to automatically relocate missing file paths.
+        Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    listener_id : str, optional
+        Specific unique ID for the TCP listener. Defaults to ``None``.
+    multi_listener : Iterable[Tuple[str, int, Optional[str]]], optional
+        Multiple remote listeners (plain TCP/IP based) to be registered at optiSLang server.
+        Each listener is a combination of host, port and (optionally) listener ID.
+        Defaults to ``None``.
     ini_timeout : float, optional
         Time in seconds to connect to the optiSLang server. The default is ``20``.
     name : str, optional
         ID of the optiSLang instance.
     password : str, optional
         Server password. The default is ``None``. This parameter is used when
         communication with the server requires that the request contain a password.
@@ -69,14 +107,53 @@
         - ``DEBUG``: Log all information for use in debugging.
 
     shutdown_on_finished: bool, optional
         Whether to shut down when execution is finished and no listeners are registered.
         The default is ``True``. This parameter is ignored when ``host`` and
         ``port`` parameters are specified.
 
+        .. note:: Only supported in batch mode.
+
+    env_vars : Mapping[str, str], optional
+        Additional environmental variables (key and value) for the optiSLang server process.
+        Defaults to ``None``.
+    import_project_properties_file : Union[str, pathlib.Path], optional
+        Optional path to a project properties file to import. Defaults to ``None``.
+    export_project_properties_file : Union[str, pathlib.Path], optional
+        Optional path to a project properties file to export. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    import_placeholders_file : Union[str, pathlib.Path], optional
+        Optional path to a placeholders file to import. Defaults to ``None``.
+    export_placeholders_file : Union[str, pathlib.Path], optional
+        Optional path to a placeholders file to export. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    output_file : Union[str, pathlib.Path], optional
+        Optional path to an output file for writing project run results to. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    dump_project_state : Union[str, pathlib.Path], optional
+        Optional path to a project state dump file to export. If a relative path is provided,
+        it is considered to be relative to the project working directory. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    opx_project_definition_file : Union[str, pathlib.Path], optional
+        Optional path to an OPX project definition file. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    additional_args : Iterable[str], optional
+        Additional command line arguments used for execution of the optiSLang server process.
+        Defaults to ``None``.
+
     Raises
     ------
     RuntimeError
         Raised when the connection to the optiSLang server cannot be established
         before the specified timeout.
 
     Examples
@@ -93,31 +170,65 @@
 
     def __init__(
         self,
         host: str = None,
         port: int = None,
         executable: Union[str, Path] = None,
         project_path: Union[str, Path] = None,
+        batch: bool = True,
+        port_range: Tuple[int, int] = None,
+        no_run: bool = None,
         no_save: bool = False,
+        force: bool = True,
+        reset: bool = False,
+        auto_relocate: bool = False,
+        listener_id: str = None,
+        multi_listener: Iterable[Tuple[str, int, Optional[str]]] = None,
         ini_timeout: Union[int, float] = 20,
         name: str = None,
         password: str = None,
         loglevel: str = None,
         shutdown_on_finished: bool = True,
+        env_vars: Mapping[str, str] = None,
+        import_project_properties_file: Union[str, Path] = None,
+        export_project_properties_file: Union[str, Path] = None,
+        import_placeholders_file: Union[str, Path] = None,
+        export_placeholders_file: Union[str, Path] = None,
+        output_file: Union[str, Path] = None,
+        dump_project_state: Union[str, Path] = None,
+        opx_project_definition_file: Union[str, Path] = None,
+        additional_args: Iterable[str] = None,
     ) -> None:
         """Initialize a new instance of the ``Optislang`` class."""
         self.__host = host
         self.__port = port
         self.__executable = Path(executable) if executable is not None else None
         self.__project_path = Path(project_path) if project_path is not None else None
+        self.__batch = batch
+        self.__port_range = port_range
+        self.__no_run = no_run
         self.__no_save = no_save
+        self.__force = force
+        self.__reset = reset
+        self.__auto_relocate = auto_relocate
         self.__ini_timeout = ini_timeout
         self.__name = name
         self.__password = password
         self.__shutdown_on_finished = shutdown_on_finished
+        self.__env_vars = env_vars
+        self.__listener_id = listener_id
+        self.__multi_listener = multi_listener
+        self.__import_project_properties_file = import_project_properties_file
+        self.__export_project_properties_file = export_project_properties_file
+        self.__import_placeholders_file = import_placeholders_file
+        self.__export_placeholders_file = export_placeholders_file
+        self.__output_file = output_file
+        self.__dump_project_state = dump_project_state
+        self.__opx_project_definition_file = opx_project_definition_file
+        self.__additional_args = additional_args
         self.__logger = LOG.add_instance_logger(self.name, self, loglevel)
         self.__osl_server: OslServer = self.__init_osl_server("tcp")
         project_uid = self.__osl_server.get_project_uid()
         self.__project = (
             Project(osl_server=self.__osl_server, uid=project_uid) if project_uid else None
         )
 
@@ -147,14 +258,31 @@
                 executable=self.__executable,
                 project_path=self.__project_path,
                 no_save=self.__no_save,
                 ini_timeout=self.__ini_timeout,
                 password=self.__password,
                 logger=self.log,
                 shutdown_on_finished=self.__shutdown_on_finished,
+                batch=self.__batch,
+                port_range=self.__port_range,
+                no_run=self.__no_run,
+                force=self.__force,
+                reset=self.__reset,
+                auto_relocate=self.__auto_relocate,
+                env_vars=self.__env_vars,
+                import_project_properties_file=self.__import_project_properties_file,
+                export_project_properties_file=self.__export_project_properties_file,
+                import_placeholders_file=self.__import_placeholders_file,
+                export_placeholders_file=self.__export_placeholders_file,
+                output_file=self.__output_file,
+                dump_project_state=self.__dump_project_state,
+                opx_project_definition_file=self.__opx_project_definition_file,
+                listener_id=self.__listener_id,
+                multi_listener=self.__multi_listener,
+                additional_args=self.__additional_args,
             )
         else:
             raise NotImplementedError(f'OptiSLang server of type "{server_type}" is not supported.')
 
     def __str__(self):
         """Return product name, version of optiSLang, and version of PyOptiSLang."""
         return (
@@ -651,14 +779,22 @@
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         self.__osl_server.stop(wait_for_finished)
 
+    def get_osl_server(self) -> Union[OslServer, None]:
+        """Get the currently used instance of the OslServer.
+
+        This instance can be used to directly communicate with optiSLang using
+        the optiSLang server API.
+        """
+        return self.__osl_server
+
     # stop_gently method doesn't work properly in optiSLang 2023 R1. Thus, it was commented out
     # def stop_gently(self, wait_for_finished: bool = True) -> None:
     #     """Stop project execution after the design is finished.
 
     #     Parameters
     #     ----------
     #     wait_for_finished : bool, optional
```

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/osl_process.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/osl_process.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 import logging
 import os
 from pathlib import Path
 import subprocess
 import tempfile
 from threading import Thread
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Sequence, Tuple, Union
+from typing import Callable, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 import psutil
 
 from ansys.optislang.core import IRON_PYTHON, encoding, utils
 
 if IRON_PYTHON:
     import System
@@ -55,43 +55,110 @@
     batch : bool, optional
         Determines whether to start optiSLang server in batch mode. Defaults to ``True``.
     port_range : Tuple[int, int], optional
         Defines the port range for optiSLang server. Defaults to ``None``.
     password : str, optional
         The server password. Use when communication with the server requires the request
         to contain a password entry. Defaults to ``None``.
+    no_run : bool, optional
+        Determines whether not to run the specified project when started in batch mode.
+        Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
     no_save : bool, optional
         Determines whether not to save the specified project after all other actions are completed.
         Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    force : bool, optional
+        Determines whether to force opening/processing specified project when started in batch mode
+        even if issues occur.
+        Defaults to ``True``.
+
+        .. note:: Only supported in batch mode.
+
+    reset : bool, optional
+        Determines whether to reset specified project after load.
+        Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    auto_relocate : bool, optional
+        Determines whether to automatically relocate missing file paths.
+        Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    enable_tcp_server : bool, optional
+        Determines whether to enable optiSLang TCP server.
+        Defaults to ``True``.
     server_info : Union[str, pathlib.Path], optional
-        Path to the server information file. If an absolute path is not supplied, it is considered
+        Path to the server information file. If a relative path is provided, it is considered
         to be relative to the project working directory. If ``None``, no server information file
         will be written. Defaults to ``None``.
     log_commands : bool, optional
         Determines whether to display server events in the Message log pane. Defaults to ``False``.
     listener : Tuple[str, int], optional
-        Host and port of the remote listener (plain TCP/IP based) to be registered by optiSLang
+        Host and port of the remote listener (plain TCP/IP based) to be registered at optiSLang
         server. Defaults to ``None``.
     listener_id : str, optional
         Specific unique ID for the TCP listener. Defaults to ``None``.
+    multi_listener : Iterable[Tuple[str, int, Optional[str]]], optional
+        Multiple remote listeners (plain TCP/IP based) to be registered at optiSLang server.
+        Each listener is a combination of host, port and (optionally) listener ID.
+        Defaults to ``None``.
     notifications : Iterable[ServerNotification], optional
         Notifications to be sent to the listener. Defaults to ``None``.
     shutdown_on_finished: bool, optional
         Shut down when execution is finished. Defaults to ``True``.
 
+        .. note:: Only supported in batch mode.
+
     env_vars : Mapping[str, str], optional
         Additional environmental variables (key and value) for the optiSLang server process.
         Defaults to ``None``.
     logger : Any, optional
         Object for logging. If ``None``, standard logging object is used. Defaults to ``None``.
     log_process_stdout : bool, optional
         Determines whether the process STDOUT is supposed to be logged. Defaults to ``True``.
     log_process_stderr : bool, optional
         Determines whether the process STDERR is supposed to be logged. Defaults to ``True``.
-    **kwargs : Dict[str, Any], optional
+    import_project_properties_file : Union[str, pathlib.Path], optional
+        Optional path to a project properties file to import. Defaults to ``None``.
+    export_project_properties_file : Union[str, pathlib.Path], optional
+        Optional path to a project properties file to export. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    import_placeholders_file : Union[str, pathlib.Path], optional
+        Optional path to a placeholders file to import. Defaults to ``None``.
+    export_placeholders_file : Union[str, pathlib.Path], optional
+        Optional path to a placeholders file to export. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    output_file : Union[str, pathlib.Path], optional
+        Optional path to an output file for writing project run results to. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    dump_project_state : Union[str, pathlib.Path], optional
+        Optional path to a project state dump file to export. If a relative path is provided,
+        it is considered to be relative to the project working directory. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    opx_project_definition_file : Union[str, pathlib.Path], optional
+        Optional path to an OPX project definition file. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    additional_args : Iterable[str], optional
         Additional command line arguments used for execution of the optiSLang server process.
         Defaults to ``None``.
 
     Raises
     ------
     TypeError
         Raised when the optiSLang executable is None.
@@ -117,94 +184,112 @@
     def __init__(
         self,
         executable: Union[str, Path] = None,
         project_path: Union[str, Path] = None,
         batch: bool = True,
         port_range: Tuple[int, int] = None,
         password: str = None,
+        no_run: bool = None,
         no_save: bool = False,
+        force: bool = True,
+        reset: bool = False,
+        auto_relocate: bool = False,
+        enable_tcp_server: bool = True,
         server_info: Union[str, Path] = None,
         log_server_events: bool = False,
         listener: Tuple[str, int] = None,
         listener_id: str = None,
+        multi_listener: Iterable[Tuple[str, int, Optional[str]]] = None,
         notifications: Iterable[ServerNotification] = None,
         shutdown_on_finished: bool = True,
         env_vars: Mapping[str, str] = None,
         logger=None,
         log_process_stdout: bool = True,
         log_process_stderr: bool = True,
-        **kwargs,
+        import_project_properties_file: Union[str, Path] = None,
+        export_project_properties_file: Union[str, Path] = None,
+        import_placeholders_file: Union[str, Path] = None,
+        export_placeholders_file: Union[str, Path] = None,
+        output_file: Union[str, Path] = None,
+        dump_project_state: Union[str, Path] = None,
+        opx_project_definition_file: Union[str, Path] = None,
+        additional_args: Iterable[str] = None,
     ) -> None:
         """Initialize a new instance of the ``OslServerProcess`` class."""
-        if logger is None:
-            self._logger = logging.getLogger(__name__)
-        else:
-            self._logger = logger
-
+        self._logger = logging.getLogger(__name__) if logger is None else logger
         self.__process = None
         self.__handle_process_output_thread = None
 
         self.__tempdir = None
 
-        if executable is not None:
-            if not os.path.isfile(executable):
-                raise FileNotFoundError(f"optiSLang executable cannot be found: {executable}")
-            self.__executable = Path(executable)
-        else:
+        if executable is None:
             osl_exec = utils.get_osl_exec()
-            if osl_exec is not None:
-                osl_version, osl_exec_path = osl_exec
-                self.__executable = osl_exec_path
-                self._logger.info(
-                    f"optiSLang executable has been found for version {osl_version} "
-                    f"on path: {osl_exec_path}"
-                )
-            else:
+            if osl_exec is None:
                 raise RuntimeError("No optiSLang executable could be found.")
 
-        if project_path == None:
-            self.__tempdir = tempfile.TemporaryDirectory()
-            project_path = Path(self.__tempdir.name) / self.__class__.DEFAULT_PROJECT_FILE
-
-        if isinstance(project_path, str):
-            project_path = Path(project_path)
-
-        if not isinstance(project_path, Path):
-            raise TypeError(
-                f"Invalid type of project_path: {type(project_path)},"
-                "Union[str, pathlib.Path] is supported."
+            osl_version, osl_exec_path = osl_exec
+            self.__executable = osl_exec_path
+            self._logger.info(
+                f"optiSLang executable has been found for version {osl_version} "
+                f"on path: {osl_exec_path}"
             )
+        elif not os.path.isfile(executable):
+            raise FileNotFoundError(f"optiSLang executable cannot be found: {executable}")
+        else:
+            self.__executable = Path(executable)
+        if batch:
+            if project_path is None:
+                self.__tempdir = tempfile.TemporaryDirectory()
+                project_path = Path(self.__tempdir.name) / self.__class__.DEFAULT_PROJECT_FILE
 
-        if not project_path.suffix == ".opf":
-            raise ValueError("Invalid optiSLang project file.")
+        self.__project_path = self.__class__.__validated_path(project_path, "project_path")
 
-        self.__project_path = project_path
+        if self.__project_path.suffix != ".opf":
+            raise ValueError("Invalid optiSLang project file.")
 
-        if isinstance(server_info, str):
-            server_info = Path(server_info)
-        elif not (isinstance(server_info, Path) or server_info is None):
-            raise TypeError(
-                f"Invalid type of server_info: {type(server_info)},"
-                "Union[str, pathlib.Path] is supported."
-            )
-        self.__server_info = server_info
+        self.__server_info = self.__class__.__validated_path(server_info, "server_info")
+        self.__import_project_properties_file = self.__class__.__validated_path(
+            import_project_properties_file, "import_project_properties_file"
+        )
+        self.__export_project_properties_file = self.__class__.__validated_path(
+            export_project_properties_file, "export_project_properties_file"
+        )
+        self.__import_placeholders_file = self.__class__.__validated_path(
+            import_placeholders_file, "import_placeholders_file"
+        )
+        self.__export_placeholders_file = self.__class__.__validated_path(
+            export_placeholders_file, "export_placeholders_file"
+        )
+        self.__output_file = self.__class__.__validated_path(output_file, "output_file")
+        self.__dump_project_state = self.__class__.__validated_path(
+            dump_project_state, "dump_project_state"
+        )
+        self.__opx_project_definition_file = self.__class__.__validated_path(
+            opx_project_definition_file, "opx_project_definition_file"
+        )
 
         self.__batch = batch
         self.__port_range = port_range
         self.__password = password
+        self.__no_run = no_run
         self.__no_save = no_save
+        self.__force = force
+        self.__reset = reset
+        self.__auto_relocate = auto_relocate
+        self.__enable_tcp_server = enable_tcp_server
         self.__log_server_events = log_server_events
         self.__listener = listener
         self.__listener_id = listener_id
+        self.__multi_listener = multi_listener
         self.__notifications = tuple(notifications) if notifications is not None else None
         self.__shutdown_on_finished = shutdown_on_finished
         self.__env_vars = dict(env_vars) if env_vars is not None else None
         self.__log_process_stdout = log_process_stdout
         self.__log_process_stderr = log_process_stderr
-        self.__additional_args = kwargs
+        self.__additional_args = additional_args
 
     @property
     def executable(self) -> Path:
         """Path to the optiSLang executable file.
 
         Returns
         -------
@@ -255,26 +340,72 @@
         -------
         str
             Server password, if defined; ``None`` otherwise.
         """
         return self.__password
 
     @property
+    def no_run(self) -> bool:
+        """Get whether not to run the specified project when started in batch mode .
+
+        Returns
+        -------
+        bool
+            ``True`` if the project is explicitly not supposed to be run;
+            ``False`` if the project is explicitly supposed to be run;
+            ``None`` otherwise.
+        """
+        return self.__no_run
+
+    @property
     def no_save(self) -> bool:
         """Get whether not to save the specified project after all other actions are completed.
 
         Returns
         -------
         bool
             ``True`` if the project is not supposed to be saved after all other actions are
             completed; ``False`` otherwise.
         """
         return self.__no_save
 
     @property
+    def reset(self) -> bool:
+        """Get whether to reset specified project after load.
+
+        Returns
+        -------
+        bool
+            ``True`` if project is to be reset after load; ``False`` otherwise.
+        """
+        return self.__reset
+
+    @property
+    def auto_relocate(self) -> bool:
+        """Get whether to automatically relocate missing file paths.
+
+        Returns
+        -------
+        bool
+            ``True`` if automatic relocation is enabled; ``False`` otherwise.
+        """
+        return self.__auto_relocate
+
+    @property
+    def enable_tcp_server(self) -> bool:
+        """Get whether to enable optiSLang TCP server.
+
+        Returns
+        -------
+        bool
+            ``True`` if optiSLang TCP server is enabled; ``False`` otherwise.
+        """
+        return self.__enable_tcp_server
+
+    @property
     def server_info(self) -> Union[Path, None]:
         """Path to the server information file.
 
         Returns
         -------
         Union[pathlib.Path, None]
             Path to the server information file, if defined; ``None`` otherwise.
@@ -293,15 +424,15 @@
         """
         return self.__log_server_events
 
     @property
     def listener(self) -> Tuple[str, int]:
         """Host and port of the remote listener.
 
-        The listener (plain TCP/IP based) is registered by optiSLang server.
+        The listener (plain TCP/IP based) is registered at optiSLang server.
 
         Returns
         -------
         Tuple[str, int]
             Host and port of the listener, if defined; ``None`` otherwise.
         """
         return self.__listener
@@ -314,14 +445,27 @@
         -------
         str
             Specific unique ID for the TCP listener, if defined; ``None`` otherwise.
         """
         return self.__listener_id
 
     @property
+    def multi_listener(self) -> Iterable[Tuple[str, int, Optional[str]]]:
+        """Multi remote listener definitions.
+
+        Aeach listener (plain TCP/IP based) is registered at optiSLang server.
+
+        Returns
+        -------
+        Iterable[Tuple[str, int, Optional[str]]]
+            Multi remote listener combinations, if defined; ``None`` otherwise.
+        """
+        return self.__multi_listener
+
+    @property
     def notifications(self) -> Tuple[ServerNotification, ...]:
         """Notifications which are sent to the listener.
 
         Returns
         -------
         Tuple[ServerNotification,...]
             Notifications which are sent to the listener, if defined; ``None`` otherwise.
@@ -371,49 +515,125 @@
         bool
             ``True`` if the STDERR of the optiSLang server process is to be logged; ``False``
             otherwise.
         """
         return self.__log_process_stderr
 
     @property
-    def additional_args(self) -> Dict[str, Any]:
+    def additional_args(self) -> Tuple[str, ...]:
         """Additional command line arguments used for optiSLang server process execution.
 
         Returns
         -------
-        Dict[str, Any]
-            Dictionary of command line arguments, if defined; ``None`` otherwise.
+        Tuple[str, ...]
+            Additional command line arguments, if defined; ``None`` otherwise.
         """
         return self.__additional_args
 
     @property
     def pid(self) -> Union[int, None]:
         """Process ID.
 
         Returns
         -------
         Union[int, None]
             Process ID, if exists; ``None`` otherwise.
         """
-        if self.__process is None:
-            return None
-
-        return self.__process.pid
+        return None if self.__process is None else self.__process.pid
 
     @property
     def shutdown_on_finished(self) -> str:
         """Whether to shut down when execution is finished.
 
         Returns
         -------
         str
             Whether to shut down when execution is finished.
         """
         return self.__shutdown_on_finished
 
+    @property
+    def import_project_properties_file(self) -> Union[Path, None]:
+        """Path to the project properties import file.
+
+        Returns
+        -------
+        Union[pathlib.Path, None]
+            Path to the project properties import file, if defined; ``None`` otherwise.
+        """
+        return self.__import_project_properties_file
+
+    @property
+    def export_project_properties_file(self) -> Union[Path, None]:
+        """Path to the project properties export file.
+
+        Returns
+        -------
+        Union[pathlib.Path, None]
+            Path to the project properties export file, if defined; ``None`` otherwise.
+        """
+        return self.__export_project_properties_file
+
+    @property
+    def import_placeholders_file(self) -> Union[Path, None]:
+        """Path to the placeholders import file.
+
+        Returns
+        -------
+        Union[pathlib.Path, None]
+            Path to the placeholders import file, if defined; ``None`` otherwise.
+        """
+        return self.__import_placeholders_file
+
+    @property
+    def export_placeholders_file(self) -> Union[Path, None]:
+        """Path to the placeholders export file.
+
+        Returns
+        -------
+        Union[pathlib.Path, None]
+            Path to the placeholders export file, if defined; ``None`` otherwise.
+        """
+        return self.__export_placeholders_file
+
+    @property
+    def output_file(self) -> Union[Path, None]:
+        """Path to the output file for writing project run results to.
+
+        Returns
+        -------
+        Union[pathlib.Path, None]
+            Path to the output file for writing project run results to, if defined;
+            ``None`` otherwise.
+        """
+        return self.__output_file
+
+    @property
+    def dump_project_state(self) -> Union[Path, None]:
+        """Path to a project state dump file to export.
+
+        Returns
+        -------
+        Union[pathlib.Path, None]
+            Path to a project state dump file to export, if defined; ``None`` otherwise.
+        """
+        return self.__dump_project_state
+
+    @property
+    def opx_project_definition_file(self) -> Union[Path, None]:
+        """Path to the OPX project definition file.
+
+        Returns
+        -------
+        Union[pathlib.Path, None]
+            Path to the OPX project definition file, if defined;
+            ``None`` otherwise.
+        """
+        return self.__opx_project_definition_file
+
     def __enter__(self):
         """Enter the context."""
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         """Exit the context."""
         self.terminate()
@@ -422,86 +642,150 @@
         """Get the command line arguments for the optiSLang server process execution.
 
         Returns
         -------
         List[str]
             List of command line arguments.
         """
-        args = []
-        args.append(str(self.__executable))
+        args = [str(self.__executable)]
 
         if self.__batch:
             args.append("-b")  # Start batch mode
 
-        if not self.__project_path.is_file():
-            # Creates a new project in the provided path.
-            if IRON_PYTHON:
-                args.append(f'--new="{str(self.__project_path)}"')
+        if self.__project_path:
+            if not self.__project_path.is_file():
+                # Creates a new project in the provided path.
+                if IRON_PYTHON:
+                    args.append(f'--new="{str(self.__project_path)}"')
+                else:
+                    args.append(f"--new={str(self.__project_path)}")
             else:
-                args.append(f"--new={str(self.__project_path)}")
-        else:
-            # Opens existing project
-            if IRON_PYTHON:
-                args.append(f'"{str(self.__project_path)}"')
-            else:
-                args.append(str(self.__project_path))
+                # Opens existing project
+                if IRON_PYTHON:
+                    args.append(f'"{str(self.__project_path)}"')
+                else:
+                    args.append(str(self.__project_path))
 
         if self.__batch:
-            args.append("--no-run")  # Does not run the specified projects.
-            # Forces projects to be processed, even if they are incomplete
-            # (can be used for damaged projects).
-            args.append("--force")
+            if self.__opx_project_definition_file:
+                if IRON_PYTHON:
+                    args.append("--python")
+                    args.append(f'"{str(utils.get_osl_opx_import_script(self.__executable))}"')
+                    args.append("--script-arg")
+                    args.append(f'"{str(self.__opx_project_definition_file)}"')
+                else:
+                    args.append("--python")
+                    args.append(str(utils.get_osl_opx_import_script(self.__executable)))
+                    args.append("--script-arg")
+                    args.append(str(self.__opx_project_definition_file))
+            if self.__no_run is None or self.__no_run:
+                # Do not run the specified projects.
+                args.append("--no-run")
+            if self.__no_save:
+                # Do not save the specified projects after all other actions have been completed.
+                args.append("--no-save")
+            if self.__force:
+                # Forces projects to be processed, even if they are incomplete
+                # (can be used for damaged projects).
+                args.append("--force")
+            if self.__shutdown_on_finished:
+                args.append("--shutdown-on-finished")
+            if self.__reset:
+                args.append("--reset")
+            if self.__auto_relocate:
+                args.append("--autorelocate")
+            if self.__export_project_properties_file is not None:
+                args.append("--export-project-properties")
+                if IRON_PYTHON:
+                    args.append(f'"{str(self.__export_project_properties_file)}"')
+                else:
+                    args.append(str(self.__export_project_properties_file))
+            if self.__export_placeholders_file is not None:
+                args.append("--export-values")
+                if IRON_PYTHON:
+                    args.append(f'"{str(self.__export_placeholders_file)}"')
+                else:
+                    args.append(str(self.__export_placeholders_file))
+            if self.__output_file is not None:
+                args.append("--output-file")
+                if IRON_PYTHON:
+                    args.append(f'"{str(self.__output_file)}"')
+                else:
+                    args.append(str(self.__output_file))
+            if self.__dump_project_state is not None:
+                if IRON_PYTHON:
+                    args.append(f'--dump-project-state="{str(self.__dump_project_state)}"')
+                else:
+                    args.append(f"--dump-project-state={str(self.__dump_project_state)}")
 
         # Enables remote surveillance (plain TCP/IP based), the port indication is optional.
-        if self.__port_range is not None:
-            args.append(f"--enable-tcp-server={self.__port_range[0]}-{self.__port_range[1]}")
-        else:
-            args.append(f"--enable-tcp-server")
+        if self.__enable_tcp_server:
+            if self.__port_range is not None:
+                args.append(f"--enable-tcp-server={self.__port_range[0]}-{self.__port_range[1]}")
+            else:
+                args.append("--enable-tcp-server")
 
         if self.__password is not None:
             # Submits the server password. Use when communication with the server requires
             # the request to contain a password entry.
             args.append(f"--server-password={self.__password}")
 
         if self.__server_info is not None:
             # Writes the server information file using the file path specified. If an absolute path
             # is not supplied, it is considered to be relative to the project working directory.
             if IRON_PYTHON:
                 args.append(f'--write-server-info="{str(self.__server_info)}"')
             else:
                 args.append(f"--write-server-info={str(self.__server_info)}")
 
-        if self.__no_save:
-            # Do not save the specified projects after all other actions have been completed.
-            args.append("--no-save")
-
-        if self.__log_server_events is not None:
+        if self.__log_server_events:
             # Displays server events in the Message log pane.
             args.append("--log-server-events")
 
         if self.__listener is not None:
             # Registers the remote listener (plain TCP/IP based) for specified host and port.
             args.append(f"--register-tcp-listener={self.__listener[0]}:{self.__listener[1]}")
 
         if self.__listener_id is not None:
             # Sets a specific unique ID for the TCP listener.
             args.append(f"--tcp-listener-id={self.__listener_id}")
 
+        if self.__multi_listener is not None:
+            if len(self.__multi_listener) >= 2:
+                args.append("--register-multi-tcp-listeners")
+            for listener in self.__multi_listener:
+                if len(listener) >= 3 and listener[2] is not None:
+                    args.append(f"{listener[0]}:{listener[1]}+{listener[2]}")
+                else:
+                    args.append(f"{listener[0]}:{listener[1]}")
+
         if self.__notifications is not None:
             # Subscribe to push notifications sent to the listener.
             args.append("--enable-notifications")
             for notification in self.__notifications:
                 args.append(notification.name)
 
+        if self.__import_project_properties_file is not None:
+            args.append("--import-project-properties")
+            if IRON_PYTHON:
+                args.append(f'"{str(self.__import_project_properties_file)}"')
+            else:
+                args.append(str(self.__import_project_properties_file))
+
+        if self.__import_placeholders_file is not None:
+            args.append("--import-values")
+            if IRON_PYTHON:
+                args.append(f'"{str(self.__import_placeholders_file)}"')
+            else:
+                args.append(str(self.__import_placeholders_file))
+
         if self.__additional_args is not None:
-            for arg_name, arg_value in self.__additional_args.items():
-                args.append(f"{arg_name}={arg_value}")
+            for arg in self.__additional_args:
+                args.append(arg)
 
-        if self.__shutdown_on_finished:
-            args.append("--shutdown-on-finished")
         return args
 
     def __remove_server_info_files(self):
         """Remove server information files.
 
         Remove all .ini files located in the same directory as optiSLang project file.
         """
@@ -674,14 +958,19 @@
             ``True`` if the optiSLang server process is running; ``False`` otherwise.
         """
         if self.__process is None:
             return False
 
         return self.__process.poll() is None
 
+    def wait_for_finished(self):
+        """Wait for the process to finish."""
+        if self.__process is not None and self.is_running():
+            self.__process.wait()
+
     def __start_process_output_thread(self):
         """Start new thread responsible for logging of STDOUT/STDERR of the optiSLang process."""
 
         def finalize_process(process, **kwargs):
             process.wait(**kwargs)
 
         self.__handle_process_output_thread = Thread(
@@ -811,7 +1100,36 @@
             threads.append(thread)
 
         for thread in threads:
             thread.join()
 
         if finalizer:
             return finalizer(process)
+
+    @staticmethod
+    def __validated_path(
+        path: Union[str, Path],
+        path_arg_name: str,
+    ):
+        """Validate a path.
+
+        Parameters
+        ----------
+        path : Union[str, pathlib.Path]
+            The path to validate.
+        path_arg_name : str
+            Path argument name/description.
+
+        Returns
+        -------
+        pathlib.Path
+            Validated path.
+        """
+        if isinstance(path, str):
+            path = Path(path)
+        elif not isinstance(path, Path) and path is not None:
+            raise TypeError(
+                f"Invalid type of {path_arg_name}: {type(path)},"
+                "Union[str, pathlib.Path] is supported."
+            )
+
+        return path
```

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/osl_server.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/osl_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,58 @@
 from pathlib import Path
 from typing import Dict, List, Sequence, Tuple, Union
 
 
 class OslServer(ABC):
     """Base class for classes which provide access to optiSLang server."""
 
+    @abstractmethod
+    def __init__(self):
+        """``OslServer`` class is an abstract base class and cannot be instantiated."""
+
+    @abstractmethod
+    def get_server_info(self) -> Dict:  # pragma: no cover
+        """Get information about the application, the server configuration and the open projects.
+
+        Returns
+        -------
+        Dict
+            Information data as dictionary.
+
+        Raises
+        ------
+        OslCommunicationError
+            Raised when an error occurs while communicating with server.
+        OslCommandError
+            Raised when the command or query fails.
+        TimeoutError
+            Raised when the timeout float value expires.
+        """
+        pass
+
+    @abstractmethod
+    def get_basic_project_info(self) -> Dict:  # pragma: no cover
+        """Get basic project info, like name, location, global settings and status.
+
+        Returns
+        -------
+        Dict
+            Information data as dictionary.
+
+        Raises
+        ------
+        OslCommunicationError
+            Raised when an error occurs while communicating with server.
+        OslCommandError
+            Raised when the command or query fails.
+        TimeoutError
+            Raised when the timeout float value expires.
+        """
+        pass
+
     # @abstractmethod
     # def close(self) -> None:
     #     """Close the current project.
 
     #     Raises
     #     ------
     #     OslCommunicationError
@@ -119,14 +163,16 @@
     def get_actor_status_info(self, uid: str, hid: str) -> Dict:  # pragma: no cover
         """Get status info of actor defined by uid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
+        hid : str
+            State/Design hierarchical id.
         Returns
         -------
         Dict
             Actor status info.
         Raises
         ------
         OslCommunicationError
@@ -280,15 +326,15 @@
         """Get input slot value of actor defined by uid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
         hid: str
-            Hid entry.
+            State/Design hierarchical id.
         slot_name: str
             Slot name.
 
         Returns
         -------
         Dict
             Input slot value of the actor.
@@ -309,15 +355,15 @@
         """Get output slot value of actor defined by uid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
         hid: str
-            Hid entry.
+            State/Design hierarchical id.
         slot_name: str
             Slot name.
 
         Returns
         -------
         Dict
             Output slot value of the actor.
@@ -900,14 +946,68 @@
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         pass
 
+    @abstractmethod
+    def get_host(self) -> Union[str, None]:  # pragma: no cover
+        """Get optiSLang server address or domain name.
+
+        Get a string representation of an IPv4/v6 address or domain name
+        of the running optiSLang server.
+
+        Returns
+        -------
+        timeout: Union[int, None]
+            The IPv4/v6 address or domain name of the running optiSLang server, if applicable.
+            Defaults to ``None``.
+        """
+        pass
+
+    @abstractmethod
+    def get_port(self) -> Union[int, None]:  # pragma: no cover
+        """Get the port the osl server is listening on.
+
+        Returns
+        -------
+        timeout: Union[int, None]
+            The port the osl server is listening on, if applicable.
+            Defaults to ``None``.
+        """
+        pass
+
+    @abstractmethod
+    def send_command(self, command: str) -> Dict:  # pragma: no cover
+        """Send command or query to the optiSLang server.
+
+        Parameters
+        ----------
+        command : str
+            Command or query to be executed on optiSLang server.
+
+        Returns
+        -------
+        Dict
+            Response from the server.
+
+        Raises
+        ------
+        RuntimeError
+            Raised when the optiSLang server is not started.
+        OslCommunicationError
+            Raised when an error occurs while communicating with server.
+        OslCommandError
+            Raised when the command or query fails.
+        TimeoutError
+            Raised when the timeout expires.
+        """
+        pass
+
     # to be fixed in 2023R2:
     # close method doesn't work properly in optiSLang 2023R1, therefore it was commented out
     # @abstractmethod
     # def close(self) -> None:  # pragma: no cover
     #     """Close the current project.
 
     #     Raises
```

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/project.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/project.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/project_parametric.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/project_parametric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1056,14 +1056,29 @@
                     value=self.limit_expression_value, value_type=self.limit_expression_value_type
                 ),
                 "type": {"value": self.criterion.name.lower()},
                 "value": Criterion._value_to_dict(value=self.value, value_type=self.value_type),
             },
         }
 
+    def __str__(self) -> str:
+        """Return information about the criterion."""
+        return (
+            f"Name: {self.name}\n"
+            f"Expression: {self.expression}\n"
+            f"Expression value: {self.expression_value}\n"
+            f"Expression value type: {self.expression_value_type}\n"
+            f"Criterion: {self.criterion}\n"
+            f"Limit expression: {self.limit_expression}\n"
+            f"Limit expression value: {self.limit_expression_value}\n"
+            f"Limit expression value type: {self.limit_expression_value_type}\n"
+            f"Value: {self.value}\n"
+            f"Value type: {self.value_type}\n"
+        )
+
 
 class LimitStateCriterion(Criterion):
     """Stores limit state criterion data."""
 
     def __init__(
         self,
         name: str = "",
@@ -1306,14 +1321,29 @@
                 "type": {
                     "value": self.criterion.name.lower(),
                 },
                 "value": Criterion._value_to_dict(value=self.value, value_type=self.value_type),
             },
         }
 
+    def __str__(self) -> str:
+        """Return information about the criterion."""
+        return (
+            f"Name: {self.name}\n"
+            f"Expression: {self.expression}\n"
+            f"Expression value: {self.expression_value}\n"
+            f"Expression value type: {self.expression_value_type}\n"
+            f"Criterion: {self.criterion}\n"
+            f"Limit expression: {self.limit_expression}\n"
+            f"Limit expression value: {self.limit_expression_value}\n"
+            f"Limit expression value type: {self.limit_expression_value_type}\n"
+            f"Value: {self.value}\n"
+            f"Value type: {self.value_type}\n"
+        )
+
 
 class ObjectiveCriterion(Criterion):
     """Stores objective criterion data."""
 
     def __init__(
         self,
         name: str = "",
@@ -1453,14 +1483,26 @@
                     self.expression_value, self.expression_value_type
                 ),
                 "type": {"value": self.criterion.name.lower()},
                 "value": Criterion._value_to_dict(self.value, self.value_type),
             },
         }
 
+    def __str__(self) -> str:
+        """Return information about the criterion."""
+        return (
+            f"Name: {self.name}\n"
+            f"Expression: {self.expression}\n"
+            f"Expression value: {self.expression_value}\n"
+            f"Expression value type: {self.expression_value_type}\n"
+            f"Criterion: {self.criterion}\n"
+            f"Value: {self.value}\n"
+            f"Value type: {self.value_type}\n"
+        )
+
 
 class VariableCriterion(Criterion):
     """Stores variable criterion data."""
 
     def __init__(
         self,
         name: str = "",
@@ -1594,14 +1636,26 @@
                     self.expression_value, self.expression_value_type
                 ),
                 "type": {"value": self.criterion.name.lower()},
                 "value": Criterion._value_to_dict(self.value, self.value_type),
             },
         }
 
+    def __str__(self) -> str:
+        """Return information about the criterion."""
+        return (
+            f"Name: {self.name}\n"
+            f"Expression: {self.expression}\n"
+            f"Expression value: {self.expression_value}\n"
+            f"Expression value type: {self.expression_value_type}\n"
+            f"Criterion: {self.criterion}\n"
+            f"Value: {self.value}\n"
+            f"Value type: {self.value_type}\n"
+        )
+
 
 # DesignVariable
 class DesignVariable:
     """Stores information about a design variable."""
 
     def __init__(
         self,
@@ -2039,14 +2093,26 @@
             "name": self.name,
             "reference_value": None,
             "removable": True,
             "type": {"value": self.type.name.lower()},
             "unit": "",
         }
 
+    def __str__(self) -> str:
+        """Return information about the parameter."""
+        return (
+            f"Name: {self.name}\n"
+            f"ID: {self.id}\n"
+            f"Reference value: {self.reference_value}\n"
+            f"Reference value type: {self.reference_value_type}\n"
+            f"Const: {self.const}\n"
+            f"Type: {self.type}\n"
+            f"Dependency expression: {self.operation}\n"
+        )
+
 
 class MixedParameter(Parameter):
     """Stores mixed parameter data."""
 
     def __init__(
         self,
         name: str = "",
@@ -2055,15 +2121,17 @@
         const: bool = False,
         deterministic_resolution: Union[ParameterResolution, str] = ParameterResolution.CONTINUOUS,
         range: Union[Sequence[float, float], Sequence[Sequence[float]]] = (-1, 1),
         stochastic_resolution: Union[
             ParameterResolution, str
         ] = ParameterResolution.MARGINALDISTRIBUTION,
         distribution_type: Union[DistributionType, str] = DistributionType.NORMAL,
-        distribution_parameters: Sequence[float] = (0, 1),
+        distribution_parameters: Union[Sequence[float], None] = None,
+        statistical_moments: Union[Sequence[float], None] = None,
+        cov: Union[float, None] = None,
     ) -> None:
         """Create a new instance of the ``MixedParameter`` class.
 
         Parameters
         ----------
         name: str
             Name of the parameter.
@@ -2077,16 +2145,20 @@
             Parameter's deterministic resolution.
         range: Union[Sequence[float, float], Sequence[Sequence[float]]], optional
             Either 2 values specifying range or list of discrete values.
         stochastic_resolution: Union[ParameterResolution, str], optional
             Parameter's stochastic resolution.
         distribution_type: Union[DistributionType, str], optional
             Parameter's distribution type.
-        distribution_parameters: Sequence[float, ...], optional
+        distribution_parameters: Union[Sequence[float, ...], None], optional
             Distribution's parameters.
+        statistical_moments: Union[Sequence[float, ...], None], optional
+            Distribution's statistical moments.
+        cov: Union[float, None], optional
+            Distribution's COV.
         """
         super().__init__(
             name=name,
             reference_value=reference_value,
             id=id,
             const=const,
             type_=ParameterType.MIXED,
@@ -2095,15 +2167,21 @@
         self.deterministic_resolution = deterministic_resolution
         if not isinstance(range[0], (float, int)):
             self.range = tuple(tuple(range[0]))
         else:
             self.range = tuple(range)
         self.stochastic_resolution = stochastic_resolution
         self.distribution_type = distribution_type
-        self.distribution_parameters = tuple(distribution_parameters)
+        self.distribution_parameters = (
+            tuple(distribution_parameters) if distribution_parameters is not None else None
+        )
+        self.statistical_moments = (
+            tuple(statistical_moments) if statistical_moments is not None else None
+        )
+        self.cov = cov
 
     def __eq__(self, other: MixedParameter) -> bool:
         """Compare properties of two instances of the ``MixedParameter`` class.
 
         Parameters
         ----------
         other: MixedParameter
@@ -2129,14 +2207,16 @@
             checks["stochastic_resolution"] = (
                 self.stochastic_resolution == other.stochastic_resolution
             )
             checks["distribution_type"] = self.distribution_type == other.distribution_type
             checks["distribution_parameters"] = (
                 self.distribution_parameters == other.distribution_parameters
             )
+            checks["statistical_moments"] = self.statistical_moments == other.statistical_moments
+            checks["cov"] = self.cov == other.cov
             return False not in checks.values()
         else:
             return False
 
     def __deepcopy__(self, memo) -> MixedParameter:
         """Return deep copy of the instance of ``MixedParameter`` class."""
         return MixedParameter(
@@ -2145,14 +2225,16 @@
             id=self.id,
             const=self.const,
             deterministic_resolution=self.deterministic_resolution,
             range=self.range,
             stochastic_resolution=self.stochastic_resolution,
             distribution_type=self.distribution_type,
             distribution_parameters=self.distribution_parameters,
+            statistical_moments=self.statistical_moments,
+            cov=self.cov,
         )
 
     @property
     def reference_value_type(self) -> ParameterValueType:
         """Type of the reference value."""
         return self.__reference_value_type
 
@@ -2261,28 +2343,66 @@
         else:
             raise TypeError(
                 "Type Union[DistributionType, str] was expected, but type: "
                 f"``{type(distribution_type)}`` was given."
             )
 
     @property
-    def distribution_parameters(self) -> Tuple[float]:
+    def distribution_parameters(self) -> Union[Tuple[float], None]:
         """Parameters of the distribution."""
         return self.__distribution_parameters
 
     @distribution_parameters.setter
-    def distribution_parameters(self, parameters: Sequence[float]):
+    def distribution_parameters(self, parameters: Union[Sequence[float], None]):
         """Set the parameters of the distribution.
 
         Parameters
         ----------
         parameters : Sequence[float]
             Parameters of the distribution.
         """
-        self.__distribution_parameters = tuple(parameters)
+        if parameters is not None:
+            self.__distribution_parameters = tuple(parameters)
+        else:
+            self.__distribution_parameters = None
+
+    @property
+    def statistical_moments(self) -> Union[Tuple[float], None]:
+        """Statistical moments of the distribution."""
+        return self.__statistical_moments
+
+    @statistical_moments.setter
+    def statistical_moments(self, moments: Union[Sequence[float], None]):
+        """Set the statistical moments of the distribution.
+
+        Parameters
+        ----------
+        moments : Sequence[float]
+            Statistical moments of the distribution.
+        """
+        if moments is not None:
+            self.__statistical_moments = tuple(moments)
+        else:
+            self.__statistical_moments = None
+
+    @property
+    def cov(self) -> Union[float, None]:
+        """COV of the distribution."""
+        return self.__cov
+
+    @cov.setter
+    def cov(self, cov: Union[float, None]):
+        """Set the statistical moments of the distribution.
+
+        Parameters
+        ----------
+        moments : Sequence[float]
+            Statistical moments of the distribution.
+        """
+        self.__cov = cov
 
     @staticmethod
     def from_dict(par_dict: dict) -> MixedParameter:
         """Create an instance of the ``MixedParameter`` class from optiSLang output.
 
         Parameters
         ----------
@@ -2315,27 +2435,45 @@
         # discrete values otherwise, stored as ([val1, val2, val3 ..])
         else:
             range = (par_dict.get("deterministic_property", {}).get("discrete_states", None),)
 
         distribution_type = DistributionType.from_str(
             par_dict.get("stochastic_property", {}).get("type", {}).get("value", None)
         )
-        distribution_parameters = tuple(
-            par_dict.get("stochastic_property", {}).get("statistical_moments", None)
+
+        distribution_parameters_from_dict = par_dict.get("stochastic_property", {}).get(
+            "distribution_parameters", None
+        )
+        if distribution_parameters_from_dict is not None:
+            distribution_parameters = tuple(distribution_parameters_from_dict)
+        else:
+            distribution_parameters = None
+
+        statistical_moments_from_dict = par_dict.get("stochastic_property", {}).get(
+            "statistical_moments", None
         )
+        if statistical_moments_from_dict is not None:
+            statistical_moments = tuple(statistical_moments_from_dict)
+        else:
+            statistical_moments = None
+
+        cov = par_dict.get("stochastic_property", {}).get("cov", None)
+
         return MixedParameter(
             name=name,
             reference_value=reference_value,
             id=id,
             const=const,
             deterministic_resolution=deterministic_resolution,
             stochastic_resolution=stochastic_resolution,
             range=range,
             distribution_type=distribution_type,
             distribution_parameters=distribution_parameters,
+            statistical_moments=statistical_moments,
+            cov=cov,
         )
 
     def to_dict(self) -> dict:
         """Convert an instance of the ``MixedParameter`` class to a dictionary.
 
         Returns
         -------
@@ -2345,38 +2483,62 @@
         if len(self.range) == 1:
             range_dict = {"discrete_states": self.range[0]}
         else:
             range_dict = {
                 "lower_bound": self.range[0],
                 "upper_bound": self.range[1],
             }
+        stochastic_property = {
+            "kind": {"value": self.stochastic_resolution.name.lower()},
+            "type": {"value": self.distribution_type.name.lower()},
+        }
+        if self.distribution_parameters is not None:
+            stochastic_property["distribution_parameters"] = self.distribution_parameters
+        if self.statistical_moments is not None:
+            stochastic_property["statistical_moments"] = self.statistical_moments
+        if self.cov is not None:
+            stochastic_property["cov"] = self.cov
         output_dict = {
             "active": True,
             "const": self.const if self.const is not None else False,
             "deterministic_property": {
                 "domain_type": {"value": self.reference_value_type.name.lower()},
                 "kind": {"value": self.deterministic_resolution.name.lower()},
             },
             "id": self.id,
             "modifiable": False,
             "name": self.name,
             "reference_value": self.reference_value if self.reference_value else 0,
             "removable": True,
-            "stochastic_property": {
-                "kind": {"value": self.stochastic_resolution.name.lower()},
-                "statistical_moments": self.distribution_parameters,
-                "type": {"value": self.distribution_type.name.lower()},
-            },
+            "stochastic_property": stochastic_property,
             "type": {"value": self.type.name.lower()},
             "unit": "",
         }
 
         output_dict["deterministic_property"].update(range_dict)
         return output_dict
 
+    def __str__(self) -> str:
+        """Return information about the parameter."""
+        return (
+            f"Name: {self.name}\n"
+            f"ID: {self.id}\n"
+            f"Reference value: {self.reference_value}\n"
+            f"Reference value type: {self.reference_value_type}\n"
+            f"Const: {self.const}\n"
+            f"Type: {self.type}\n"
+            f"Deterministic resolution: {self.deterministic_resolution}\n"
+            f"Range: {self.range}\n"
+            f"Stochastic_resolution: {self.stochastic_resolution}\n"
+            f"Distribution type: {self.distribution_type}\n"
+            f"Distribution parameters: {self.distribution_parameters}\n"
+            f"Statistical moments: {self.statistical_moments}\n"
+            f"COV: {self.cov}\n"
+        )
+
 
 class OptimizationParameter(Parameter):
     """Stores optimization parameter data."""
 
     def __init__(
         self,
         name: str = "",
@@ -2612,29 +2774,44 @@
             "removable": True,
             "type": {"value": self.type.name.lower()},
             "unit": "",
         }
         output_dict["deterministic_property"].update(range_dict)
         return output_dict
 
+    def __str__(self) -> str:
+        """Return information about the parameter."""
+        return (
+            f"Name: {self.name}\n"
+            f"ID: {self.id}\n"
+            f"Reference value: {self.reference_value}\n"
+            f"Reference value type: {self.reference_value_type}\n"
+            f"Const: {self.const}\n"
+            f"Type: {self.type}\n"
+            f"Deterministic resolution: {self.deterministic_resolution}\n"
+            f"Range: {self.range}\n"
+        )
+
 
 class StochasticParameter(Parameter):
     """Stores stochastic parameter data."""
 
     def __init__(
         self,
         name: str = "",
         reference_value: Union[bool, float, str, None] = 0,
         id: str = str(uuid.uuid4()),
         const: bool = False,
         stochastic_resolution: Union[
             ParameterResolution, str
         ] = ParameterResolution.MARGINALDISTRIBUTION,
         distribution_type: Union[DistributionType, str] = DistributionType.NORMAL,
-        distribution_parameters: Sequence[float] = (0, 1),
+        distribution_parameters: Union[Sequence[float], None] = None,
+        statistical_moments: Union[Sequence[float], None] = None,
+        cov: Union[float, None] = None,
     ) -> None:
         """Create a new instance of the ``StochasticParameter`` class.
 
         Parameters
         ----------
         name: str
             Name of the parameter.
@@ -2644,28 +2821,38 @@
             Parameter's unique id.
         const: bool, optional
             Determines whether is parameter constant.
         stochastic_resolution: Union[ParameterResolution, str], optional
             Parameter's stochastic resolution.
         distribution_type: Union[DistributionType, str], optional
             Parameter's distribution type.
-        distribution_parameters: Sequence[float], optional
+        distribution_parameters: Union[Sequence[float, ...], None], optional
             Distribution's parameters.
+        statistical_moments: Union[Sequence[float, ...], None], optional
+            Distribution's statistical moments.
+        cov: Union[float, None], optional
+            Distribution's COV.
         """
         super().__init__(
             name=name,
             reference_value=reference_value,
             id=id,
             const=const,
             type_=ParameterType.STOCHASTIC,
         )
         self.__reference_value_type = ParameterValueType.REAL
         self.stochastic_resolution = stochastic_resolution
         self.distribution_type = distribution_type
-        self.distribution_parameters = tuple(distribution_parameters)
+        self.distribution_parameters = (
+            tuple(distribution_parameters) if distribution_parameters is not None else None
+        )
+        self.statistical_moments = (
+            tuple(statistical_moments) if statistical_moments is not None else None
+        )
+        self.cov = cov
 
     def __eq__(self, other: StochasticParameter) -> bool:
         r"""Compare properties of two instances of the ``StochasticParameter`` class.
 
         Parameters
         ----------
         other: StochasticParameter
@@ -2687,28 +2874,32 @@
             checks["stochastic_resolution"] = (
                 self.stochastic_resolution == other.stochastic_resolution
             )
             checks["distribution_type"] = self.distribution_type == other.distribution_type
             checks["distribution_parameters"] = (
                 self.distribution_parameters == other.distribution_parameters
             )
+            checks["statistical_moments"] = self.statistical_moments == other.statistical_moments
+            checks["cov"] = self.cov == other.cov
             return False not in checks.values()
         else:
             return False
 
     def __deepcopy__(self, memo) -> StochasticParameter:
         """Return deep copy of the stochastic parameter."""
         return StochasticParameter(
             name=self.name,
             reference_value=self.reference_value,
             id=self.id,
             const=self.const,
             stochastic_resolution=self.stochastic_resolution,
             distribution_type=self.distribution_type,
             distribution_parameters=self.distribution_parameters,
+            statistical_moments=self.statistical_moments,
+            cov=self.cov,
         )
 
     @property
     def reference_value_type(self) -> ParameterValueType:
         """Type of the reference value``."""
         return self.__reference_value_type
 
@@ -2767,28 +2958,66 @@
         else:
             raise TypeError(
                 "Type Union[DistributionType, str] was expected, but type: "
                 f"``{type(distribution_type)}`` was given."
             )
 
     @property
-    def distribution_parameters(self) -> Tuple[float]:
+    def distribution_parameters(self) -> Union[Tuple[float], None]:
         """Parameters of the distribution."""
         return self.__distribution_parameters
 
     @distribution_parameters.setter
-    def distribution_parameters(self, parameters: Sequence[float]) -> None:
+    def distribution_parameters(self, parameters: Union[Sequence[float], None]):
         """Set the parameters of the distribution.
 
         Parameters
         ----------
         parameters : Sequence[float]
             Parameters of the distribution.
         """
-        self.__distribution_parameters = tuple(parameters)
+        if parameters is not None:
+            self.__distribution_parameters = tuple(parameters)
+        else:
+            self.__distribution_parameters = None
+
+    @property
+    def statistical_moments(self) -> Union[Tuple[float], None]:
+        """Statistical moments of the distribution."""
+        return self.__statistical_moments
+
+    @statistical_moments.setter
+    def statistical_moments(self, moments: Union[Sequence[float], None]):
+        """Set the statistical moments of the distribution.
+
+        Parameters
+        ----------
+        moments : Sequence[float]
+            Statistical moments of the distribution.
+        """
+        if moments is not None:
+            self.__statistical_moments = tuple(moments)
+        else:
+            self.__statistical_moments = None
+
+    @property
+    def cov(self) -> Union[float, None]:
+        """COV of the distribution."""
+        return self.__cov
+
+    @cov.setter
+    def cov(self, cov: Union[float, None]):
+        """Set the statistical moments of the distribution.
+
+        Parameters
+        ----------
+        moments : Sequence[float]
+            Statistical moments of the distribution.
+        """
+        self.__cov = cov
 
     @staticmethod
     def from_dict(par_dict: dict) -> StochasticParameter:
         """Create an instance of the ``StochasticParameter`` class from the optiSLang server output.
 
         Parameters
         ----------
@@ -2806,52 +3035,88 @@
         const = par_dict["const"]
         stochastic_resolution = ParameterResolution.from_str(
             par_dict.get("stochastic_property", {}).get("kind", {}).get("value", None)
         )
         distribution_type = DistributionType.from_str(
             par_dict.get("stochastic_property", {}).get("type", {}).get("value", None)
         )
-        distribution_parameters = tuple(
-            par_dict.get("stochastic_property", {}).get("statistical_moments", None)
+        distribution_parameters_from_dict = par_dict.get("stochastic_property", {}).get(
+            "distribution_parameters", None
         )
+        if distribution_parameters_from_dict is not None:
+            distribution_parameters = tuple(distribution_parameters_from_dict)
+        else:
+            distribution_parameters = None
+        statistical_moments_from_dict = par_dict.get("stochastic_property", {}).get(
+            "statistical_moments", None
+        )
+        if statistical_moments_from_dict is not None:
+            statistical_moments = tuple(statistical_moments_from_dict)
+        else:
+            statistical_moments = None
+        cov = par_dict.get("stochastic_property", {}).get("cov", None)
         return StochasticParameter(
             name=name,
             reference_value=reference_value,
             id=id,
             const=const,
             stochastic_resolution=stochastic_resolution,
             distribution_type=distribution_type,
             distribution_parameters=distribution_parameters,
+            statistical_moments=statistical_moments,
+            cov=cov,
         )
 
     def to_dict(self) -> dict:
         """Convert an instance of the ``StochasticParameter`` to dictionary.
 
         Returns
         -------
         dict
             Input dictionary for the optiSLang server.
         """
+        stochastic_property = {
+            "kind": {"value": self.stochastic_resolution.name.lower()},
+            "type": {"value": self.distribution_type.name.lower()},
+        }
+        if self.distribution_parameters is not None:
+            stochastic_property["distribution_parameters"] = self.distribution_parameters
+        if self.statistical_moments is not None:
+            stochastic_property["statistical_moments"] = self.statistical_moments
+        if self.cov is not None:
+            stochastic_property["cov"] = self.cov
         return {
             "active": True,
             "const": self.const if self.const is not None else False,
             "id": self.id,
             "modifiable": False,
             "name": self.name,
             "reference_value": self.reference_value,
             "removable": True,
-            "stochastic_property": {
-                "kind": {"value": self.stochastic_resolution.name.lower()},
-                "statistical_moments": self.distribution_parameters,
-                "type": {"value": self.distribution_type.name.lower()},
-            },
+            "stochastic_property": stochastic_property,
             "type": {"value": self.type.name.lower()},
             "unit": "",
         }
 
+    def __str__(self) -> str:
+        """Return information about the parameter."""
+        return (
+            f"Name: {self.name}\n"
+            f"ID: {self.id}\n"
+            f"Reference value: {self.reference_value}\n"
+            f"Reference value type: {self.reference_value_type}\n"
+            f"Const: {self.const}\n"
+            f"Type: {self.type}\n"
+            f"Stochastic_resolution: {self.stochastic_resolution}\n"
+            f"Distribution type: {self.distribution_type}\n"
+            f"Distribution parameters: {self.distribution_parameters}\n"
+            f"Statistical moments: {self.statistical_moments}\n"
+            f"COV: {self.cov}\n"
+        )
+
 
 # Response
 class Response:
     """Stores response data."""
 
     def __init__(
         self,
@@ -3060,14 +3325,22 @@
 
         """
         return {
             "name": self.name,
             "reference_value": self.reference_value,
         }
 
+    def __str__(self) -> str:
+        """Return information about the response."""
+        return (
+            f"Name: {self.name}\n"
+            f"Reference value: {self.reference_value}\n"
+            f"Reference value type: {self.reference_value_type}\n"
+        )
+
 
 # MANAGERS:
 
 
 class CriteriaManager:
     """Contains methods for obtaining criteria."""
```

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/server_commands.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/server_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,14 +587,15 @@
 def register_listener(
     id: str = None,
     host: str = None,
     port: int = None,
     timeout: int = None,
     notifications: Iterable[str] = None,
     password: str = None,
+    listener_uid: str = None,
 ) -> str:
     """Generate JSON string of register_listener command.
 
     Parameters
     ----------
     id: str, opt
         Id of the local listener.
@@ -604,14 +605,16 @@
         Port of the TCP listener.
     time_out: int, opt
         Unregister policy timeout in ms, default 60000 ms.
     notifications: Sequence, opt
         Notifications.
     password : str, opt
         Password.
+    listener_uid : str, opt
+        Listener UID.
 
     Returns
     -------
     str
         JSON string of register_listener command.
     """
     args = {}
@@ -625,14 +628,16 @@
         args["host"] = host
         args["port"] = port
 
     if timeout is not None:
         args["timeout"] = timeout
     if notifications is not None:
         args["notifications"] = notifications
+    if listener_uid is not None:
+        args["uid"] = listener_uid
 
     return _to_json(_gen_server_command(command=_REGISTER_LISTENER, args=args, password=password))
 
 
 def register_locations_as_parameter(actor_uid: str, password: str = None) -> str:
     """Generate JSON string of ``register_location_as_parameter`` command.
 
@@ -1151,15 +1156,15 @@
 
     Parameters
     ----------
     type_: str
         Argument type,
         for application dialogs: [ "about", "help", "settings", "plugin" ]
         for project dialogs: [ "project_settings", "project_overview", "license_management",
-            "registered_files", "purge", "load_from", "save_to" ].
+        "registered_files", "purge", "load_from", "save_to" ].
     usage_mode: str, opt
         Usage mode. e.g. "EXPERT".
     parent_hwnd: str, opt
         Parent hwnd.
     password : str, opt
         Password.
 
@@ -1335,17 +1340,17 @@
     uid: str
         Uid entry.
     notifications: Sequence
         Either ["ALL"] or Sequence picked from below options:
             Server: [ "SERVER_UP", "SERVER_DOWN" ] (always be sent by default).
             Logging: [ "LOG_INFO", "LOG_WARNING", "LOG_ERROR", "LOG_DEBUG" ].
             Project: [ "EXECUTION_STARTED", "PROCESSING_STARTED", "EXECUTION_FINISHED",
-                "NOTHING_PROCESSED", "CHECK_FAILED", "EXEC_FAILED" ].
+            "NOTHING_PROCESSED", "CHECK_FAILED", "EXEC_FAILED" ].
             Nodes: [ "ACTOR_STATE_CHANGED", "ACTOR_ACTIVE_CHANGED", "ACTOR_NAME_CHANGED",
-                "ACTOR_CONTENTS_CHANGED", "ACTOR_DATA_CHANGED" ].
+            ACTOR_CONTENTS_CHANGED", "ACTOR_DATA_CHANGED" ].
     node_types: Sequence, opt
        Node types, e.g. ["Sensitivity", "AnsysWorkbench"].
     password : str, opt
         Password.
 
     Returns
     -------
```

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/server_queries.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/server_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/tcp_osl_server.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/tcp_osl_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from datetime import datetime
 import json
 import logging
 import os
 from pathlib import Path
 from queue import Queue
 import re
-import select
 import signal
 import socket
 import struct
 import threading
 import time
-from typing import Callable, Dict, List, Sequence, Tuple, Union
+from typing import Callable, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 import uuid
 
 from ansys.optislang.core import server_commands as commands
 from ansys.optislang.core import server_queries as queries
 from ansys.optislang.core.encoding import force_bytes, force_text
 from ansys.optislang.core.errors import (
     ConnectionEstablishedError,
@@ -396,37 +395,25 @@
             raise ValueError("Timeout value must be greater than zero or None.")
 
         start_time = time.time()
         self.__socket.settimeout(timeout)
 
         response_len = -1
         bytes_to_receive = self.__class__._RESPONSE_SIZE_BYTES
+
         # read from socket until response size (twice) has been received
-        while True:
-            try:
-                # Test if we will be able to read something from the connection.
-                readable_sockets, _, _ = select.select([self.__socket], [], [], 1)
-                if self.__socket in readable_sockets:
-                    # Read and convert response size. Assume server sent response size twice.
-                    # Sizes need to match.
-                    response_len_1 = struct.unpack("!Q", self.__socket.recv(bytes_to_receive))[0]
-                    response_len_2 = struct.unpack("!Q", self.__socket.recv(bytes_to_receive))[0]
-                    if response_len_1 != response_len_2:
-                        raise ResponseFormatError("The message size values do not match.")
+        response_len_1 = struct.unpack("!Q", self._receive_bytes(bytes_to_receive, timeout))[0]
+        response_len_2 = struct.unpack("!Q", self._receive_bytes(bytes_to_receive, timeout))[0]
 
-                    response_len = response_len_1
-                if response_len >= 0:
-                    break
-            except Exception as e:
-                self._logger.debug(e)
-                pass
-            now = time.time()
-            elapsed = now - start_time
-            if timeout is not None and elapsed > timeout:
-                raise TimeoutError("Time to receive message length has expired.")
+        if response_len_1 != response_len_2:
+            raise ResponseFormatError(
+                "Server response format unrecognized. Response sizes do not match."
+            )
+
+        response_len = response_len_1
 
         return response_len
 
     def _receive_bytes(self, count: int, timeout: Union[float, None]) -> bytes:
         """Receive specified number of bytes from the server.
 
         Parameters
@@ -553,14 +540,15 @@
         Raised when port_range not type Tuple[int, int]
     TimeoutError
         Raised when the timeout float value expires.
 
     Examples
     --------
     Create listener
+
     >>> from ansys.optislang.core.tcp_osl_server import TcpOslListener
     >>> general_listener = TcpOslListener(
     >>>     port_range = (49152, 65535),
     >>>     timeout = 30,
     >>>     name = 'GeneralListener',
     >>>     host = '127.0.0.1',
     >>>     uid = str(uuid.uuid4()),
@@ -803,14 +791,21 @@
                 if client is not None:
                     client.disconnect()
 
 
 class TcpOslServer(OslServer):
     """Class which provides access to optiSLang server using plain TCP/IP communication protocol.
 
+    TcpOslServer class provides explicit methods for accessing specific optiSLang API endpoints.
+    Additionally, the generic
+    :mod:`send_command <ansys.optislang.core.tcp_osl_server.TcpOslServer.send_command>` method
+    can be used in conjunction with the convenience functions from the
+    :ref:`ansys.optislang.core.server_queries <ref_osl_server_api_queries>` and
+    :ref:`ansys.optislang.core.server_commands <ref_osl_server_api_commands>` modules.
+
     For remote connection, it is assumed that the optiSLang server process is already running
     on remote (or local) host. In that case, the host and port must be specified and other
     parameters are ignored.
 
     Parameters
     ----------
     host : str, optional
@@ -824,47 +819,126 @@
     project_path : Union[str, pathlib.Path], optional
         Path to the optiSLang project file which is supposed to be used by new local optiSLang
         server. It is ignored when the host and port parameters are specified.
         - If the project file exists, it is opened.
         - If the project file does not exist, a new project is created on the specified path.
         - If the path is None, a new project is created in the temporary directory.
         Defaults to ``None``.
+    batch : bool, optional
+        Determines whether to start optiSLang server in batch mode. Defaults to ``True``.
+    port_range : Tuple[int, int], optional
+        Defines the port range for optiSLang server. Defaults to ``None``.
+    no_run : bool, optional
+        Determines whether not to run the specified project when started in batch mode.
+        Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
     no_save : bool, optional
         Determines whether not to save the specified project after all other actions are completed.
         It is ignored when the host and port parameters are specified. Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    force : bool, optional
+        Determines whether to force opening/processing specified project when started in batch mode
+        even if issues occur.
+        Defaults to ``True``.
+
+        .. note:: Only supported in batch mode.
+
+    reset : bool, optional
+        Determines whether to reset specified project after load.
+        Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    auto_relocate : bool, optional
+        Determines whether to automatically relocate missing file paths.
+        Defaults to ``False``.
+
+        .. note:: Only supported in batch mode.
+
+    listener_id : str, optional
+        Specific unique ID for the TCP listener. Defaults to ``None``.
+    multi_listener : Iterable[Tuple[str, int, Optional[str]]], optional
+        Multiple remote listeners (plain TCP/IP based) to be registered at optiSLang server.
+        Each listener is a combination of host, port and (optionally) listener ID.
+        Defaults to ``None``.
     ini_timeout : float, optional
         Time in seconds to listen to the optiSLang server port. If the port is not listened
         for specified time, the optiSLang server is not started and RuntimeError is raised.
         It is ignored when the host and port parameters are specified. Defaults to 20 s.
     password : str, optional
         The server password. Use when communication with the server requires the request
         to contain a password entry. Defaults to ``None``.
     logger : Any, optional
         Object for logging. If ``None``, standard logging object is used. Defaults to ``None``.
     shutdown_on_finished: bool, optional
         Shut down when execution is finished and there are not any listeners registered.
         It is ignored when the host and port parameters are specified. Defaults to ``True``.
 
+        .. note:: Only supported in batch mode.
+
+    env_vars : Mapping[str, str], optional
+        Additional environmental variables (key and value) for the optiSLang server process.
+        Defaults to ``None``.
+    import_project_properties_file : Union[str, pathlib.Path], optional
+        Optional path to a project properties file to import. Defaults to ``None``.
+    export_project_properties_file : Union[str, pathlib.Path], optional
+        Optional path to a project properties file to export. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    import_placeholders_file : Union[str, pathlib.Path], optional
+        Optional path to a placeholders file to import. Defaults to ``None``.
+    export_placeholders_file : Union[str, pathlib.Path], optional
+        Optional path to a placeholders file to export. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    output_file : Union[str, pathlib.Path], optional
+        Optional path to an output file for writing project run results to. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    dump_project_state : Union[str, pathlib.Path], optional
+        Optional path to a project state dump file to export. If a relative path is provided,
+        it is considered to be relative to the project working directory. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    opx_project_definition_file : Union[str, pathlib.Path], optional
+        Optional path to an OPX project definition file. Defaults to ``None``.
+
+        .. note:: Only supported in batch mode.
+
+    additional_args : Iterable[str], optional
+        Additional command line arguments used for execution of the optiSLang server process.
+        Defaults to ``None``.
+
     Raises
     ------
     RuntimeError
         Port listener cannot be started.
         -or-
         optiSLang server port is not listened for specified timeout value.
 
     Examples
     --------
     Start local optiSLang server, get optiSLang version and shutdown the server.
+
     >>> from ansys.optislang.core.tcp_osl_server import TcpOslServer
     >>> osl_server = TcpOslServer()
     >>> osl_version = osl_server.get_osl_version_string()
     >>> print(osl_version)
     >>> osl_server.shutdown()
 
     Connect to the remote optiSLang server, get optiSLang version and shutdown the server.
+
     >>> from ansys.optislang.core.tcp_osl_server import TcpOslServer
     >>> host = "192.168.101.1"  # IP address of the remote host
     >>> port = 49200            # Port of the remote optiSLang server
     >>> osl_server = TcpOslServer(host, port)
     >>> osl_version = osl_server.get_osl_version_string()
     >>> print(osl_version)
     >>> osl_server.shutdown()
@@ -887,52 +961,88 @@
 
     def __init__(
         self,
         host: str = None,
         port: int = None,
         executable: Union[str, Path] = None,
         project_path: Union[str, Path] = None,
+        batch: bool = True,
+        port_range: Tuple[int, int] = None,
+        no_run: bool = None,
         no_save: bool = False,
+        force: bool = True,
+        reset: bool = False,
+        auto_relocate: bool = False,
+        listener_id: str = None,
+        multi_listener: Iterable[Tuple[str, int, Optional[str]]] = None,
         ini_timeout: float = 20,
         password: str = None,
         logger=None,
         shutdown_on_finished=True,
+        env_vars: Mapping[str, str] = None,
+        import_project_properties_file: Union[str, Path] = None,
+        export_project_properties_file: Union[str, Path] = None,
+        import_placeholders_file: Union[str, Path] = None,
+        export_placeholders_file: Union[str, Path] = None,
+        output_file: Union[str, Path] = None,
+        dump_project_state: Union[str, Path] = None,
+        opx_project_definition_file: Union[str, Path] = None,
+        additional_args: Iterable[str] = None,
     ) -> None:
         """Initialize a new instance of the ``TcpOslServer`` class."""
         self.__host = host
         self.__port = port
         self.__timeout = None
 
         if logger is None:
             self._logger = logging.getLogger(__name__)
         else:
             self._logger = logger
 
         self.__executable = Path(executable) if executable is not None else None
         self.__project_path = Path(project_path) if project_path is not None else None
+        self.__batch = batch
+        self.__port_range = port_range
+        self.__no_run = no_run
         self.__no_save = no_save
+        self.__force = force
+        self.__reset = reset
+        self.__auto_relocate = auto_relocate
         self.__password = password
         self.__osl_process = None
         self.__listeners = {}
         self.__listeners_registration_thread = None
         self.__refresh_listeners = threading.Event()
         self.__listeners_refresh_interval = 20
         self.__disposed = False
+        self.__env_vars = env_vars
+        self.__listener_id = listener_id
+        self.__multi_listener = multi_listener
+        self.__import_project_properties_file = import_project_properties_file
+        self.__export_project_properties_file = export_project_properties_file
+        self.__import_placeholders_file = import_placeholders_file
+        self.__export_placeholders_file = export_placeholders_file
+        self.__output_file = output_file
+        self.__dump_project_state = dump_project_state
+        self.__opx_project_definition_file = opx_project_definition_file
+        self.__additional_args = additional_args
+
         signal.signal(signal.SIGINT, self.__signal_handler)
         atexit.register(self.dispose)
 
         if self.__host is None or self.__port is None:
             self.__host = self.__class__._LOCALHOST
             self.__shutdown_on_finished = shutdown_on_finished
             self._start_local(ini_timeout, shutdown_on_finished)
         else:
             self.__shutdown_on_finished = None
             listener = self.__create_listener(
                 timeout=self.__timeout,
                 name="Main",
+                uid=self.__listener_id,
             )
             listener.uid = self.__register_listener(
                 host=listener.host,
                 port=listener.port,
                 notifications=[
                     ServerNotification.SERVER_UP,
                     ServerNotification.SERVER_DOWN,
@@ -947,15 +1057,15 @@
         if osl_version[0] is not None:
             if osl_version[0] < 23:
                 self._logger.warning(
                     f"The version of the used Ansys optiSLang ({osl_version_string})"
                     " is not fully supported. Please use at least version 23.1."
                 )
 
-    def _get_server_info(self) -> Dict:
+    def get_server_info(self) -> Dict:
         """Get information about the application, the server configuration and the open projects.
 
         Returns
         -------
         Dict
             Information data as dictionary.
 
@@ -964,17 +1074,17 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.server_info(self.__password))
+        return self.send_command(queries.server_info(self.__password))
 
-    def _get_basic_project_info(self) -> Dict:
+    def get_basic_project_info(self) -> Dict:
         """Get basic project info, like name, location, global settings and status.
 
         Returns
         -------
         Dict
             Information data as dictionary.
 
@@ -983,15 +1093,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.basic_project_info(self.__password))
+        return self.send_command(queries.basic_project_info(self.__password))
 
     def dispose(self) -> None:
         """Terminate all local threads and unregister listeners.
 
         Raises
         ------
         OslCommunicationError
@@ -1027,15 +1137,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             commands.evaluate_design(evaluate_dict, self.__password),
         )
 
     def get_actor_info(self, uid: str) -> Dict:
         """Get info about actor defined by uid.
 
         Parameters
@@ -1053,15 +1163,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.actor_info(uid=uid, password=self.__password))
+        return self.send_command(queries.actor_info(uid=uid, password=self.__password))
 
     def get_actor_states(self, uid: str) -> Dict:
         """Get available actor states for a certain actor (only the IDs of the available states).
 
         These can be used in conjunction with "get_actor_status_info" to obtain actor status info
         for a specific state ID.
 
@@ -1078,39 +1188,39 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.actor_states(uid=uid, password=self.__password))
+        return self.send_command(queries.actor_states(uid=uid, password=self.__password))
 
     def get_actor_status_info(self, uid: str, hid: str) -> Dict:
         """Get status info about actor defined by actor uid and state Hid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
         hid: str
-            Hid entry.
+            State/Design hierarchical id.
         Returns
         -------
         Dict
             Info about actor defined by uid.
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             queries.actor_status_info(uid=uid, hid=hid, password=self.__password)
         )
 
     def get_actor_supports(self, uid: str, feature_name: str) -> bool:
         """Get supported features of actor defined by uid.
 
         Parameters
@@ -1130,15 +1240,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             queries.actor_supports(uid=uid, feature_name=feature_name, password=self.__password)
         )[feature_name.lower()]
 
     def get_actor_properties(self, uid: str) -> Dict:
         """Get properties of actor defined by uid.
 
         Parameters
@@ -1156,15 +1266,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.actor_properties(uid=uid, password=self.__password))
+        return self.send_command(queries.actor_properties(uid=uid, password=self.__password))
 
     def get_full_project_status_info(self) -> Dict:
         """Get full project status info.
 
         Returns
         -------
         Dict
@@ -1175,15 +1285,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.full_project_status_info(password=self.__password))
+        return self.send_command(queries.full_project_status_info(password=self.__password))
 
     def get_full_project_tree(self) -> Dict:
         """Get full project tree.
 
         Returns
         -------
         Dict
@@ -1194,15 +1304,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.full_project_tree(password=self.__password))
+        return self.send_command(queries.full_project_tree(password=self.__password))
 
     def get_full_project_tree_with_properties(self) -> Dict:
         """Get full project tree with properties.
 
         Returns
         -------
         Dict
@@ -1213,15 +1323,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             queries.full_project_tree_with_properties(password=self.__password)
         )
 
     def get_hpc_licensing_forwarded_environment(self, uid: str) -> Dict:
         """Get hpc licensing forwarded environment for certain actor.
 
         Parameters
@@ -1239,27 +1349,27 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             queries.hpc_licensing_forwarded_environment(uid=uid, password=self.__password)
         )
 
     def get_input_slot_value(self, uid: str, hid: str, slot_name: str) -> Dict:
         """Get input slot value of actor defined by uid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
         hid: str
-            Hid entry.
+            State/Design hierarchical id.
         slot_name: str
             Slot name.
 
         Returns
         -------
         Dict
             Input slot value of the actor.
@@ -1269,29 +1379,29 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             queries.input_slot_value(
                 uid=uid, hid=hid, slot_name=slot_name, password=self.__password
             )
         )
 
     def get_output_slot_value(self, uid: str, hid: str, slot_name: str) -> Dict:
         """Get output slot value of actor defined by uid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
         hid: str
-            Hid entry.
+            State/Design hierarchical id.
         slot_name: str
             Slot name.
 
         Returns
         -------
         Dict
             Output slot value of the actor.
@@ -1301,15 +1411,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             queries.output_slot_value(
                 uid=uid, hid=hid, slot_name=slot_name, password=self.__password
             )
         )
 
     def get_osl_version_string(self) -> str:
         """Get version of used optiSLang.
@@ -1324,15 +1434,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        server_info = self._get_server_info()
+        server_info = self.get_server_info()
         return server_info["application"]["version"]
 
     def get_osl_version(self) -> Tuple[Union[int, None], ...]:
         """Get version of used optiSLang.
 
         Returns
         -------
@@ -1395,15 +1505,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        project_info = self._get_basic_project_info()
+        project_info = self.get_basic_project_info()
         if len(project_info.get("projects", [])) == 0:
             return None
         return (
             project_info.get("projects", [{}])[0].get("settings", {}).get("short_description", None)
         )
 
     def get_project_location(self) -> Path:
@@ -1420,15 +1530,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        project_info = self._get_basic_project_info()
+        project_info = self.get_basic_project_info()
         project_path = project_info.get("projects", [{}])[0].get("location", None)
         return None if not project_path else Path(project_path)
 
     def get_project_name(self) -> str:
         """Get name of the optiSLang project.
 
         Returns
@@ -1442,15 +1552,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        project_info = self._get_basic_project_info()
+        project_info = self.get_basic_project_info()
         if len(project_info.get("projects", [])) == 0:
             return None
         return project_info.get("projects", [{}])[0].get("name", None)
 
     def get_project_status(self) -> str:
         """Get status of the optiSLang project.
 
@@ -1465,15 +1575,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        project_info = self._get_basic_project_info()
+        project_info = self.get_basic_project_info()
         if len(project_info.get("projects", [])) == 0:
             return None
         return project_info.get("projects", [{}])[0].get("state", None)
 
     def get_project_uid(self) -> str:
         """Get project uid.
 
@@ -1508,15 +1618,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.project_tree_systems(password=self.__password))
+        return self.send_command(queries.project_tree_systems(password=self.__password))
 
     def get_project_tree_systems_with_properties(self) -> Dict:
         """Get project tree systems with properties.
 
         Returns
         -------
         Dict
@@ -1527,15 +1637,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(
+        return self.send_command(
             queries.project_tree_systems_with_properties(password=self.__password)
         )
 
     def get_server_is_alive(self) -> bool:
         """Get info whether the server is alive.
 
         Returns
@@ -1548,15 +1658,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        response_dict = self._send_command(queries.server_is_alive(password=self.__password))
+        response_dict = self.send_command(queries.server_is_alive(password=self.__password))
         is_alive = response_dict.get("status") == "success"
         return is_alive
 
     def get_systems_status_info(self) -> Dict:
         """Get project status info, including systems only.
 
         Returns
@@ -1569,15 +1679,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        return self._send_command(queries.systems_status_info(password=self.__password))
+        return self.send_command(queries.systems_status_info(password=self.__password))
 
     def get_timeout(self) -> Union[float, None]:
         """Get current timeout value for execution of commands.
 
         Returns
         -------
         timeout: Union[float, None]
@@ -1608,15 +1718,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        project_info = self._get_basic_project_info()
+        project_info = self.get_basic_project_info()
         if len(project_info.get("projects", [])) == 0:
             return None
         return Path(project_info.get("projects", [{}])[0].get("working_dir", None))
 
     def new(self) -> None:
         """Create a new project.
 
@@ -1625,15 +1735,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        self._send_command(commands.new(password=self.__password))
+        self.send_command(commands.new(password=self.__password))
 
     def open(
         self,
         file_path: Union[str, Path],
         force: bool = True,
         restore: bool = False,
         reset: bool = False,
@@ -1665,15 +1775,15 @@
         """
         file_path = self.__cast_to_path(file_path=file_path)
         self.__validate_path(file_path=file_path)
 
         if not file_path.is_file():
             raise FileNotFoundError(f'File "{file_path}" doesn\'t exist.')
 
-        self._send_command(
+        self.send_command(
             commands.open(
                 path=str(file_path.as_posix()),
                 do_force=force,
                 do_restore=restore,
                 do_reset=reset,
                 password=self.__password,
             )
@@ -1687,15 +1797,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        self._send_command(commands.reset(password=self.__password))
+        self.send_command(commands.reset(password=self.__password))
 
     def run_python_script(
         self,
         script: str,
         args: Union[Sequence[object], None] = None,
     ) -> Tuple[str, str]:
         """Load a Python script in a project context and execute it.
@@ -1717,15 +1827,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        responses = self._send_command(commands.run_python_script(script, args, self.__password))
+        responses = self.send_command(commands.run_python_script(script, args, self.__password))
         std_out = ""
         std_err = ""
         for response in responses:
             std_out += response.get("std_out", "")
             std_err += response.get("std_err", "")
 
         return (std_out, std_err)
@@ -1776,15 +1886,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        self._send_command(commands.save(password=self.__password))
+        self.send_command(commands.save(password=self.__password))
 
     def save_as(
         self,
         file_path: Union[str, Path],
         force: bool = True,
         restore: bool = False,
         reset: bool = False,
@@ -1813,15 +1923,15 @@
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         file_path = self.__cast_to_path(file_path=file_path)
         self.__validate_path(file_path=file_path)
 
-        self._send_command(
+        self.send_command(
             commands.save_as(
                 path=str(file_path.as_posix()),
                 do_force=force,
                 do_restore=restore,
                 do_reset=reset,
                 password=self.__password,
             )
@@ -1842,15 +1952,15 @@
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         file_path = self.__cast_to_path(file_path=file_path)
         self.__validate_path(file_path=file_path)
-        self._send_command(commands.save_copy(str(file_path.as_posix()), self.__password))
+        self.send_command(commands.save_copy(str(file_path.as_posix()), self.__password))
 
     def set_timeout(self, timeout: Union[float, None] = None) -> None:
         """Set timeout value for execution of commands.
 
         Parameters
         ----------
         timeout: Union[float, None]
@@ -1918,15 +2028,15 @@
         """
         self.__stop_listeners_registration_thread()
         self.__unregister_all_listeners()
         self.__dispose_all_listeners()
 
         if self.__shutdown_on_finished in (False, None):
             try:
-                self._send_command(commands.shutdown(self.__password))
+                self.send_command(commands.shutdown(self.__password))
             except Exception:
                 if not force or self.__osl_process is None:
                     raise
 
         # If desired actively force osl process to terminate
         if force and self.__osl_process is not None:
             self._force_shutdown_local_process()
@@ -2017,15 +2127,15 @@
                     self._logger,
                 ),
             )
             exec_finished_listener.start_listening()
             self._logger.debug("Wait for finished thread was created.")
 
         if not already_running:
-            self._send_command(commands.start(self.__password))
+            self.send_command(commands.start(self.__password))
 
         if not already_running and (wait_for_started or wait_for_finished):
             self._logger.info(f"Waiting for started")
             successfully_started = wait_for_started_queue.get()
             self.__delete_exec_started_listener()
             if successfully_started == "Terminate":
                 raise TimeoutError("Waiting for started timed out.")
@@ -2088,28 +2198,53 @@
                 exec_finished_listener.clear_callbacks()
                 self.__delete_exec_finished_listener()
             return
         elif status in self._STOP_REQUESTS_PRIORITIES:
             stop_request_priority = self._STOP_REQUESTS_PRIORITIES["STOP"]
             current_status_priority = self._STOP_REQUESTED_STATES_PRIORITIES[status]
             if stop_request_priority > current_status_priority:
-                self._send_command(commands.stop(self.__password))
+                self.send_command(commands.stop(self.__password))
             else:
                 self._logger.debug(f"Do not send STOP request, project status is: {status}")
         else:
-            self._send_command(commands.stop(self.__password))
+            self.send_command(commands.stop(self.__password))
 
         if wait_for_finished:
             self._logger.info(f"Waiting for finished")
             successfully_finished = wait_for_finished_queue.get()
             self.__delete_exec_finished_listener()
             if successfully_finished == "Terminate":
                 raise TimeoutError("Waiting for finished timed out.")
             self._logger.info(f"Successfully_finished: {successfully_finished}.")
 
+    def get_host(self) -> Union[str, None]:
+        """Get optiSLang server address or domain name.
+
+        Get a string representation of an IPv4/v6 address or domain name
+        of the running optiSLang server.
+
+        Returns
+        -------
+        timeout: Union[int, None]
+            The IPv4/v6 address or domain name of the running optiSLang server, if applicable.
+            Defaults to ``None``.
+        """
+        return self.__host
+
+    def get_port(self) -> Union[int, None]:
+        """Get the port the osl server is listening on.
+
+        Returns
+        -------
+        timeout: Union[int, None]
+            The port the osl server is listening on, if applicable.
+            Defaults to ``None``.
+        """
+        return self.__port
+
     def _unregister_listener(self, listener: TcpOslListener) -> None:
         """Unregister a listener.
 
         Parameters
         ----------
         listener : TcpOslListener
             Class with listener properties.
@@ -2119,15 +2254,15 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        self._send_command(commands.unregister_listener(str(listener.uid), self.__password))
+        self.send_command(commands.unregister_listener(str(listener.uid), self.__password))
         listener.uid = None
 
     def _start_local(self, ini_timeout: float, shutdown_on_finished: bool) -> None:
         """Start local optiSLang server.
 
         Parameters
         ----------
@@ -2146,35 +2281,53 @@
             -or-
             optiSLang server port is not listened for specified timeout value.
         """
         if self.__osl_process is not None:
             raise RuntimeError("optiSLang server is already started.")
 
         listener = self.__create_listener(
-            uid=str(uuid.uuid4()), timeout=self.__timeout, name="Main"
+            uid=self.__listener_id if self.__listener_id else str(uuid.uuid4()),
+            timeout=self.__timeout,
+            name="Main",
         )
         port_queue = Queue()
         listener.add_callback(self.__class__.__port_on_listended, (port_queue, self._logger))
 
         try:
             listener.start_listening(timeout=ini_timeout)
 
             self.__osl_process = OslServerProcess(
                 executable=self.__executable,
                 project_path=self.__project_path,
                 no_save=self.__no_save,
                 password=self.__password,
                 listener=(listener.host, listener.port),
                 listener_id=listener.uid,
+                multi_listener=self.__multi_listener,
                 notifications=[
                     ServerNotification.SERVER_UP,
                     ServerNotification.SERVER_DOWN,
                 ],
                 shutdown_on_finished=shutdown_on_finished,
                 logger=self._logger,
+                batch=self.__batch,
+                port_range=self.__port_range,
+                no_run=self.__no_run,
+                force=self.__force,
+                reset=self.__reset,
+                auto_relocate=self.__auto_relocate,
+                env_vars=self.__env_vars,
+                import_project_properties_file=self.__import_project_properties_file,
+                export_project_properties_file=self.__export_project_properties_file,
+                import_placeholders_file=self.__import_placeholders_file,
+                export_placeholders_file=self.__export_placeholders_file,
+                output_file=self.__output_file,
+                dump_project_state=self.__dump_project_state,
+                opx_project_definition_file=self.__opx_project_definition_file,
+                additional_args=self.__additional_args,
             )
             self.__osl_process.start()
 
             listener.join()
             if not port_queue.empty():
                 self.__port = port_queue.get()
 
@@ -2379,21 +2532,22 @@
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        msg = self._send_command(
+        msg = self.send_command(
             commands.register_listener(
                 host=host,
                 port=port,
                 timeout=timeout,
                 notifications=[ntf.name for ntf in notifications],
                 password=self.__password,
+                listener_uid=self.__listener_id,
             )
         )
         return msg[0]["uid"]
 
     def __refresh_listeners_registration(self) -> None:  # pragma: no cover
         """Refresh listeners registration.
 
@@ -2410,15 +2564,15 @@
         """
         check_for_refresh = 0.5
         counter = 0
         while self.__refresh_listeners.is_set():
             if counter >= self.__listeners_refresh_interval:
                 for listener in self.__listeners.values():
                     if listener.refresh_listener_registration:
-                        response = self._send_command(
+                        response = self.send_command(
                             commands.refresh_listener_registration(
                                 uid=listener.uid, password=self.__password
                             )
                         )
                 counter = 0
             counter += check_for_refresh
             time.sleep(check_for_refresh)
@@ -2452,15 +2606,15 @@
         if not isinstance(file_path, Path):
             raise TypeError(
                 f'Invalid type of project_path: "{type(file_path)}", "pathlib.Path" is supported.'
             )
         if not file_path.suffix == ".opf":
             raise ValueError('Invalid optiSLang project file, project must end with ".opf".')
 
-    def _send_command(self, command: str) -> Dict:
+    def send_command(self, command: str) -> Dict:
         """Send command or query to the optiSLang server.
 
         Parameters
         ----------
         command : str
             Command or query to be executed on optiSLang server.
 
@@ -2527,15 +2681,15 @@
     #     OslCommunicationError
     #         Raised when an error occurs while communicating with server.
     #     OslCommandError
     #         Raised when the command or query fails.
     #     TimeoutError
     #         Raised when the timeout float value expires.
     #     """
-    #     self._send_command(commands.close(password=self.__password))
+    #     self.send_command(commands.close(password=self.__password))
 
     # stop_gently method doesn't work properly in optiSLang 2023R1, therefore it was commented out
     # def stop_gently(self, wait_for_finished: bool = True) -> None:
     #     """Stop project execution after the current design is finished.
 
     #     Parameters
     #     ----------
@@ -2583,19 +2737,19 @@
     #             exec_finished_listener.clear_callbacks()
     #             self.__delete_exec_finished_listener()
     #         return
     #     elif status in self._STOP_REQUESTS_PRIORITIES:
     #         stop_request_priority = self._STOP_REQUESTS_PRIORITIES["STOP_GENTLY"]
     #         current_status_priority = self._STOP_REQUESTED_STATES_PRIORITIES[status]
     #         if stop_request_priority > current_status_priority:
-    #             self._send_command(commands.stop(self.__password))
+    #             self.send_command(commands.stop(self.__password))
     #         else:
     #             self._logger.debug(f"Do not send STOP request, project status is: {status}")
     #     else:
-    #         self._send_command(commands.stop(self.__password))
+    #         self.send_command(commands.stop(self.__password))
 
     #     if wait_for_finished:
     #         self._logger.info(f"Waiting for finished")
     #         successfully_finished = wait_for_finished_queue.get()
     #         self.__delete_exec_finished_listener()
     #         if successfully_finished == "Terminate":
     #             raise TimeoutError("Waiting for finished timed out.")
```

### Comparing `ansys_optislang_core-0.2.1/src/ansys/optislang/core/utils.py` & `ansys_optislang_core-0.3.0/src/ansys/optislang/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import collections
 from enum import Enum
 import os
 from pathlib import Path
 import re
-from typing import Dict, Iterable, OrderedDict, Tuple, Union
+from typing import Dict, Iterable, Optional, OrderedDict, Tuple, Union
 
 from ansys.optislang.core import FIRST_SUPPORTED_VERSION
 
 
 def enum_from_str(
     string: str, enum_class: Enum, replace: Union[Tuple[str, str], None] = None
 ) -> Enum:
@@ -111,14 +111,47 @@
     elif os.name == "posix":
         return _find_all_osl_exec_in_posix()
     # another os
     else:
         raise NotImplementedError(f"Unsupported OS {os.name}.")
 
 
+def get_osl_opx_import_script(osl_executable: Union[str, Path] = None) -> Optional[Path]:
+    """Get the path to the optiSLang OPX import script file.
+
+    Parameters
+    ----------
+    osl_executable : Union[str, pathlib.Path], optional
+        optiSLang executable path to use as a reference for locating the import script file.
+        The default is ``None``, in which case the default optiSLang executable file is used.
+
+    Returns
+    -------
+    Tuple[int, pathlib.Path], None
+        Path to the optiSLang OPX import script file, if location succeeded,
+        ``None`` is returned otherwise.
+
+    Raises
+    ------
+    NotImplementedError
+        Raised when the operating system is not supported.
+    """
+    if osl_executable is None:
+        osl_executable = get_osl_exec()[1]
+
+    if osl_executable is not None:
+        osl_opx_import_script_path = (
+            osl_executable.parent / "tools" / "import" / "opx" / "convert_opx_to_opf.py"
+        )
+        if osl_opx_import_script_path.is_file():
+            return osl_opx_import_script_path
+
+    return None
+
+
 def _find_all_osl_exec_in_windows() -> OrderedDict[int, Tuple[Path, ...]]:
     """Find all optiSLang executable files on Windows.
 
     Returns
     -------
     OrderedDict[int, Tuple[Path, ...]]
         Ordered dictionary of found optiSLang executables. The dictionary key corresponds
```

### Comparing `ansys_optislang_core-0.2.1/PKG-INFO` & `ansys_optislang_core-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-optislang-core
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python wrapper for Ansys optiSLang application.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -17,24 +17,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: importlib-metadata>=4.0,<7
 Requires-Dist: psutil>=5.9
 Requires-Dist: build>=0.8.0 ; extra == "build"
 Requires-Dist: twine>=4.0.1 ; extra == "build"
-Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
-Requires-Dist: Sphinx==7.0.0 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinxcontrib-images==0.9.4 ; extra == "doc"
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: matplotlib>=3.5.3 ; extra == "tests"
 Project-URL: Documentation, https://optislang.docs.pyansys.com
 Project-URL: Homepage, https://optislang.docs.pyansys.com
 Project-URL: Source, https://github.com/pyansys/pyoptislang
 Project-URL: Tracker, https://github.com/pyansys/pyoptislang/issues
 Provides-Extra: build
 Provides-Extra: doc
@@ -79,15 +79,15 @@
 --------
 PyOptiSLang is a Python wrapper for Ansys optiSLang. It supports Pythonic
 access to Ansys optiSLang to be able to communicate with Ansys optiSLang directly from Python.
 The latest ``ansys-optislang`` package provides these capabilities:
 
 - Starting and managing local instances of Ansys optiSLang
 - Remote connections to Ansys optiSLang instances via TCP/IP
-- Create new Ansys optiSLang project	
+- Create new Ansys optiSLang project
 - Open existing Ansys optiSLang project
 - Control Ansys optiSLang project execution
 - Save Ansys optiSLang project
 - Execute classic Ansys optiSLang Python API script on backend side
 - Evaluate designs on root project level
```

