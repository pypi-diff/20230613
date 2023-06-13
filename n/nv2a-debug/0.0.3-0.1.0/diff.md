# Comparing `tmp/nv2a_debug-0.0.3.tar.gz` & `tmp/nv2a_debug-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nv2a_debug-0.0.3.tar", last modified: Mon Jun 27 03:26:49 2022, max compression
+gzip compressed data, was "nv2a_debug-0.1.0.tar", last modified: Tue Jun 13 14:04:35 2023, max compression
```

## Comparing `nv2a_debug-0.0.3.tar` & `nv2a_debug-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.392360 nv2a_debug-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2022-06-27 03:26:49.392360 nv2a_debug-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4498 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/build_cffi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.380360 nv2a_debug-0.0.3/nv2a_debug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2022-06-27 03:26:49.000000 nv2a_debug-0.0.3/nv2a_debug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-06-27 03:26:49.000000 nv2a_debug-0.0.3/nv2a_debug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 03:26:49.000000 nv2a_debug-0.0.3/nv2a_debug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-27 03:26:49.000000 nv2a_debug-0.0.3/nv2a_debug.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-27 03:26:49.000000 nv2a_debug-0.0.3/nv2a_debug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-27 03:26:49.000000 nv2a_debug-0.0.3/nv2a_debug.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.384360 nv2a_debug-0.0.3/nv2adbg/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/nv2adbg/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    33960 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/nv2adbg/debugger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/nv2adbg/py_nv2a_vsh_emu.py
--rw-r--r--   0 runner    (1001) docker     (121)     6501 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/nv2adbg/simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-06-27 03:26:49.392360 nv2a_debug-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      252 2022-06-27 03:26:44.000000 nv2a_debug-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.376360 nv2a_debug-0.0.3/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.384360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/.git
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.376360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.384360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.384360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/githooks/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3097 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/githooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.388360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/
--rw-r--r--   0 runner    (1001) docker     (121)     8195 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h
--rw-r--r--   0 runner    (1001) docker     (121)    11975 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c
--rw-r--r--   0 runner    (1001) docker     (121)     4429 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h
--rw-r--r--   0 runner    (1001) docker     (121)     5954 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.376360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.388360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/disassembler/
--rw-r--r--   0 runner    (1001) docker     (121)    21365 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/disassembler/test_main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.388360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/emulator/
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/emulator/test_main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 03:26:49.392360 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/operations/
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-27 03:26:45.000000 nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/operations/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/build_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/src/nv2adbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_code_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_file_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_input_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_output_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_program_inputs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_program_outputs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_register_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_shader_program.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8132 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/py_nv2a_vsh_emu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/tests/test__code_panel_build_ancestor_root_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/tests/test__code_panel_build_contributing_source_segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/githooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3097 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/githooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/test_main.cpp
```

### Comparing `nv2a_debug-0.0.3/LICENSE` & `nv2a_debug-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/build_cffi.py` & `nv2a_debug-0.1.0/build_cffi.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/nv2adbg/py_nv2a_vsh_emu.py` & `nv2a_debug-0.1.0/src/nv2adbg/py_nv2a_vsh_emu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 from _nv2a_vsh_cpu import ffi
 from _nv2a_vsh_cpu import lib
 
 _OPCODES = [
     "NOP",
     "MOV",
@@ -50,15 +50,16 @@
     ".xzw",
     ".xy",
     ".xyw",
     ".xyz",
     "",  # ".xyzw",
 ]
 
-_OUTPUT_NAMES = {
+"""Maps output register indices to names (e.g., o3: oD0)"""
+OUTPUT_NAMES = {
     0: "oPos",
     3: "oD0",
     4: "oD1",
     5: "oFog",
     6: "oPts",
     7: "oB0",
     8: "oB1",
@@ -74,15 +75,15 @@
 def _stringify_output(type, index, writemask) -> str:
     mask = _WRITEMASKS[writemask]
 
     if type == lib.NV2ART_CONTEXT:
         return f"c[{index}]{mask}"
 
     if type == lib.NV2ART_OUTPUT:
-        return f"{_OUTPUT_NAMES[index]}{mask}"
+        return f"{OUTPUT_NAMES[index]}{mask}"
 
     return f"{_REGISTERS[type]}{index}{mask}"
 
 
 def _make_swizzle(components: List[int]) -> str:
     if components == [0, 1, 2, 3]:
         return ""
@@ -94,15 +95,14 @@
 
     components = [_SWIZZLES[val] for val in components]
     swizzle_str = "".join(components)
     return f".{swizzle_str}"
 
 
 def _stringify_input(type, index, swizzle, negate: bool, relative: bool) -> str:
-
     if type == lib.NV2ART_CONTEXT:
         rel = "A0+" if relative else ""
         reg = f"c[{rel}{index}]"
     else:
         reg = _REGISTERS[type] + str(index)
 
     # Expand the FFI array into a list for easier manipulation.
@@ -244,7 +244,30 @@
             ret["temp"] = retrieve_regs("R", self._state.temp_regs, 12)
             ret["output"] = retrieve_regs("o", self._state.output_regs, 13)
 
         return ret
 
     def apply(self, step: Nv2aVshStep):
         lib.nv2a_vsh_emu_apply(ffi.addressof(self._token), step._step)
+
+    def get_register_value(self, name: str) -> Tuple[float, float, float, float]:
+        """Returns the current value of the given register."""
+
+        def _get(destination, reg_name):
+            index = int(reg_name[1:]) * 4
+            return tuple(destination[index : index + 4])
+
+        if name == "oPos":
+            name = "R12"
+
+        if name[0] == "v":
+            return _get(self._state.input_regs, name)
+        if name[0] == "c":
+            return _get(self._state.context_regs, name)
+        if name[0] == "R":
+            return _get(self._state.temp_regs, name)
+        if name[0] == "o":
+            return _get(self._state.output_regs, name)
+        if name == "A0":
+            return tuple(self._state.address_reg)
+
+        raise Exception(f"Unknown register '{name}'")
```

### Comparing `nv2a_debug-0.0.3/setup.cfg` & `nv2a_debug-0.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nv2a_debug
-version = 0.0.3
+version = 0.1.0
 author = Erik Abair
 author_email = erik.abair@bearbrains.work
 description = Simulator/debugger for the Xbox nv2a vertex shader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/abaire/nv2a_vsh_debug
 project_urls = 
@@ -15,24 +15,28 @@
 	License :: OSI Approved :: The Unlicense (Unlicense)
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Programming Language :: Assembly
 	Topic :: Software Development :: Debuggers
 
 [options]
+package_dir = 
+	=src
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.9
 include_package_data = True
 install_requires = 
 	nv2a-vsh >= 0.1.1
-	rich
-	sshkeyboard
 	cffi
+	textual >= 0.27.0
 setup_requires = cffi
 
+[options.packages.find]
+where = src
+
 [options.entry_points]
 console_scripts = 
 	nv2adbg = nv2adbg:run
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/CMakeLists.txt` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/LICENSE` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/LICENSE`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/githooks/pre-commit` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/githooks/pre-commit`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.0.3/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp` & `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp`

 * *Files identical despite different names*

