# Comparing `tmp/cocotb-1.7.2.tar.gz` & `tmp/cocotb-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocotb-1.7.2.tar", last modified: Tue Nov 15 21:06:19 2022, max compression
+gzip compressed data, was "cocotb-1.8.0rc1.tar", last modified: Mon Jun 12 21:37:16 2023, max compression
```

## Comparing `cocotb-1.7.2.tar` & `cocotb-1.8.0rc1.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.694496 cocotb-1.7.2/
--rw-r--r--   0 runner     (501) staff       (20)     1542 2022-11-15 20:52:47.000000 cocotb-1.7.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      131 2022-11-15 20:52:47.000000 cocotb-1.7.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     6118 2022-11-15 21:06:19.694665 cocotb-1.7.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4985 2022-11-15 20:52:47.000000 cocotb-1.7.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.658423 cocotb-1.7.2/cocotb/
--rw-r--r--   0 runner     (501) staff       (20)     3366 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/ANSI.py
--rw-r--r--   0 runner     (501) staff       (20)    11662 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1153 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_deprecation.py
--rw-r--r--   0 runner     (501) staff       (20)     2691 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_py_compat.py
--rw-r--r--   0 runner     (501) staff       (20)     2835 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_sim_versions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.662240 cocotb-1.7.2/cocotb/_vendor/
--rw-r--r--   0 runner     (501) staff       (20)     1166 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/README.md
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12839 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/distutils_version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.663864 cocotb-1.7.2/cocotb/_vendor/fli/
--rw-r--r--   0 runner     (501) staff       (20)    25349 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/fli/acc_user.h
--rw-r--r--   0 runner     (501) staff       (20)    11914 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/fli/acc_vhdl.h
--rw-r--r--   0 runner     (501) staff       (20)    32939 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/fli/mti.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.666360 cocotb-1.7.2/cocotb/_vendor/tcl/
--rw-r--r--   0 runner     (501) staff       (20)     2255 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/tcl/license.terms
--rw-r--r--   0 runner     (501) staff       (20)    94743 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/tcl/tcl.h
--rw-r--r--   0 runner     (501) staff       (20)   169681 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/tcl/tclDecls.h
--rw-r--r--   0 runner     (501) staff       (20)     3279 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/tcl/tclPlatDecls.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.666875 cocotb-1.7.2/cocotb/_vendor/vhpi/
--rw-r--r--   0 runner     (501) staff       (20)    42107 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/vhpi/vhpi_user.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.667984 cocotb-1.7.2/cocotb/_vendor/vpi/
--rw-r--r--   0 runner     (501) staff       (20)    25694 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/vpi/sv_vpi_user.h
--rw-r--r--   0 runner     (501) staff       (20)    44349 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_vendor/vpi/vpi_user.h
--rw-r--r--   0 runner     (501) staff       (20)      295 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/_version.py
--rwxr-xr-x   0 runner     (501) staff       (20)    26172 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/binary.py
--rw-r--r--   0 runner     (501) staff       (20)     6436 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/clock.py
--rwxr-xr-x   0 runner     (501) staff       (20)     9847 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/config.py
--rw-r--r--   0 runner     (501) staff       (20)    20749 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/decorators.py
--rwxr-xr-x   0 runner     (501) staff       (20)    41612 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/handle.py
--rw-r--r--   0 runner     (501) staff       (20)     2828 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/ipython_support.py
--rw-r--r--   0 runner     (501) staff       (20)    10443 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/log.py
--rw-r--r--   0 runner     (501) staff       (20)     1853 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/memdebug.py
--rw-r--r--   0 runner     (501) staff       (20)     1299 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/outcomes.py
--rw-r--r--   0 runner     (501) staff       (20)     5159 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/queue.py
--rw-r--r--   0 runner     (501) staff       (20)    32636 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/regression.py
--rw-r--r--   0 runner     (501) staff       (20)     6696 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/result.py
--rw-r--r--   0 runner     (501) staff       (20)    31641 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)    40302 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/scheduler.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.642723 cocotb-1.7.2/cocotb/share/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.670956 cocotb-1.7.2/cocotb/share/def/
--rw-r--r--   0 runner     (501) staff       (20)       44 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/def/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      376 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/def/README.md
--rw-r--r--   0 runner     (501) staff       (20)      930 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/def/aldec.def
--rw-r--r--   0 runner     (501) staff       (20)      662 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/def/ghdl.def
--rw-r--r--   0 runner     (501) staff       (20)      655 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/def/icarus.def
--rw-r--r--   0 runner     (501) staff       (20)     2214 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/def/modelsim.def
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.674683 cocotb-1.7.2/cocotb/share/include/
--rw-r--r--   0 runner     (501) staff       (20)     3998 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/cocotb_utils.h
--rw-r--r--   0 runner     (501) staff       (20)     2520 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/embed.h
--rw-r--r--   0 runner     (501) staff       (20)      657 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/exports.h
--rw-r--r--   0 runner     (501) staff       (20)    10051 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/gpi.h
--rw-r--r--   0 runner     (501) staff       (20)    10341 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/gpi_logging.h
--rw-r--r--   0 runner     (501) staff       (20)      642 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/py_gpi_logging.h
--rw-r--r--   0 runner     (501) staff       (20)      628 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/vhpi_user_ext.h
--rw-r--r--   0 runner     (501) staff       (20)     2374 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/include/vpi_user_ext.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.642510 cocotb-1.7.2/cocotb/share/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.675612 cocotb-1.7.2/cocotb/share/lib/embed/
--rw-r--r--   0 runner     (501) staff       (20)     4422 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/embed/embed.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10454 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/embed/gpi_embed.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.677666 cocotb-1.7.2/cocotb/share/lib/fli/
--rw-r--r--   0 runner     (501) staff       (20)     7255 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/fli/FliCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    39423 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/fli/FliImpl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15344 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/fli/FliImpl.h
--rw-r--r--   0 runner     (501) staff       (20)    26438 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/fli/FliObjHdl.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.679203 cocotb-1.7.2/cocotb/share/lib/gpi/
--rw-r--r--   0 runner     (501) staff       (20)     4679 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/gpi/GpiCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    19525 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/gpi/GpiCommon.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10685 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/gpi/gpi_priv.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.679665 cocotb-1.7.2/cocotb/share/lib/gpi_log/
--rw-r--r--   0 runner     (501) staff       (20)     7056 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/gpi_log/gpi_logging.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.680124 cocotb-1.7.2/cocotb/share/lib/py_gpi_log/
--rw-r--r--   0 runner     (501) staff       (20)     7022 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.680592 cocotb-1.7.2/cocotb/share/lib/simulator/
--rw-r--r--   0 runner     (501) staff       (20)    41171 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/simulator/simulatormodule.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.681154 cocotb-1.7.2/cocotb/share/lib/utils/
--rw-r--r--   0 runner     (501) staff       (20)     3896 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/utils/cocotb_utils.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.681614 cocotb-1.7.2/cocotb/share/lib/verilator/
--rw-r--r--   0 runner     (501) staff       (20)     4145 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/verilator/verilator.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.683165 cocotb-1.7.2/cocotb/share/lib/vhpi/
--rw-r--r--   0 runner     (501) staff       (20)    38559 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/vhpi/VhpiCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    35763 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/vhpi/VhpiImpl.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9989 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/vhpi/VhpiImpl.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.684691 cocotb-1.7.2/cocotb/share/lib/vpi/
--rw-r--r--   0 runner     (501) staff       (20)    27082 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/vpi/VpiCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    22067 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/vpi/VpiImpl.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9661 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/lib/vpi/VpiImpl.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.686118 cocotb-1.7.2/cocotb/share/makefiles/
--rw-r--r--   0 runner     (501) staff       (20)      416 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/Makefile.deprecations
--rw-r--r--   0 runner     (501) staff       (20)     6498 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/Makefile.inc
--rw-r--r--   0 runner     (501) staff       (20)     5281 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/Makefile.sim
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.691102 cocotb-1.7.2/cocotb/share/makefiles/simulators/
--rw-r--r--   0 runner     (501) staff       (20)     2656 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.activehdl
--rw-r--r--   0 runner     (501) staff       (20)     3901 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.cvc
--rw-r--r--   0 runner     (501) staff       (20)     3542 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.ghdl
--rw-r--r--   0 runner     (501) staff       (20)     3847 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.icarus
--rw-r--r--   0 runner     (501) staff       (20)     4451 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.ius
--rw-r--r--   0 runner     (501) staff       (20)     1906 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.modelsim
--rw-r--r--   0 runner     (501) staff       (20)     6364 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.questa
--rw-r--r--   0 runner     (501) staff       (20)     5815 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.riviera
--rw-r--r--   0 runner     (501) staff       (20)     3589 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.vcs
--rw-r--r--   0 runner     (501) staff       (20)     2286 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.verilator
--rw-r--r--   0 runner     (501) staff       (20)     5315 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.xcelium
--rw-r--r--   0 runner     (501) staff       (20)    31636 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/triggers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.693338 cocotb-1.7.2/cocotb/types/
--rw-r--r--   0 runner     (501) staff       (20)     1803 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10899 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/types/array.py
--rw-r--r--   0 runner     (501) staff       (20)     8499 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/types/logic.py
--rw-r--r--   0 runner     (501) staff       (20)     9063 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/types/logic_array.py
--rw-r--r--   0 runner     (501) staff       (20)     6230 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/types/range.py
--rw-r--r--   0 runner     (501) staff       (20)    23064 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     5988 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/wavedrom.py
--rw-r--r--   0 runner     (501) staff       (20)     3552 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb/xunit_reporter.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.660953 cocotb-1.7.2/cocotb.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     6118 2022-11-15 21:06:19.000000 cocotb-1.7.2/cocotb.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3088 2022-11-15 21:06:19.000000 cocotb-1.7.2/cocotb.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-11-15 21:06:19.000000 cocotb-1.7.2/cocotb.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       53 2022-11-15 21:06:19.000000 cocotb-1.7.2/cocotb.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)       33 2022-11-15 21:06:19.000000 cocotb-1.7.2/cocotb.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)      516 2022-11-15 21:06:19.000000 cocotb-1.7.2/cocotb.egg-info/top_level.txt
--rwxr-xr-x   0 runner     (501) staff       (20)    27213 2022-11-15 20:52:47.000000 cocotb-1.7.2/cocotb_build_libs.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-15 21:06:19.694068 cocotb-1.7.2/pygpi/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-11-15 20:52:47.000000 cocotb-1.7.2/pygpi/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      946 2022-11-15 20:52:47.000000 cocotb-1.7.2/pygpi/entry.py
--rw-r--r--   0 runner     (501) staff       (20)     2089 2022-11-15 20:52:47.000000 cocotb-1.7.2/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      726 2022-11-15 21:06:19.695461 cocotb-1.7.2/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     5543 2022-11-15 20:52:47.000000 cocotb-1.7.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.508607 cocotb-1.8.0rc1/
+-rw-r--r--   0 runner     (501) staff       (20)     1542 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      131 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     6717 2023-06-12 21:37:16.508825 cocotb-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     5581 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.459431 cocotb-1.8.0rc1/cocotb/
+-rw-r--r--   0 runner     (501) staff       (20)     3366 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/cocotb/ANSI.py
+-rw-r--r--   0 runner     (501) staff       (20)    11296 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1153 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_deprecation.py
+-rw-r--r--   0 runner     (501) staff       (20)     2691 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_py_compat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3544 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_sim_versions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.464655 cocotb-1.8.0rc1/cocotb/_vendor/
+-rw-r--r--   0 runner     (501) staff       (20)     1166 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/README.md
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12839 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/distutils_version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.466487 cocotb-1.8.0rc1/cocotb/_vendor/fli/
+-rw-r--r--   0 runner     (501) staff       (20)    25349 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_user.h
+-rw-r--r--   0 runner     (501) staff       (20)    11914 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_vhdl.h
+-rw-r--r--   0 runner     (501) staff       (20)    32939 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/fli/mti.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.469758 cocotb-1.8.0rc1/cocotb/_vendor/tcl/
+-rw-r--r--   0 runner     (501) staff       (20)     2255 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/license.terms
+-rw-r--r--   0 runner     (501) staff       (20)    94743 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/tcl.h
+-rw-r--r--   0 runner     (501) staff       (20)   169681 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclDecls.h
+-rw-r--r--   0 runner     (501) staff       (20)     3279 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclPlatDecls.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.470460 cocotb-1.8.0rc1/cocotb/_vendor/vhpi/
+-rw-r--r--   0 runner     (501) staff       (20)    42107 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/vhpi/vhpi_user.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.472031 cocotb-1.8.0rc1/cocotb/_vendor/vpi/
+-rw-r--r--   0 runner     (501) staff       (20)    25694 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/vpi/sv_vpi_user.h
+-rw-r--r--   0 runner     (501) staff       (20)    44349 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/vpi/vpi_user.h
+-rw-r--r--   0 runner     (501) staff       (20)      298 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/_version.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    26172 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/binary.py
+-rw-r--r--   0 runner     (501) staff       (20)     6560 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/clock.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     9847 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/config.py
+-rw-r--r--   0 runner     (501) staff       (20)    11476 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/decorators.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    41612 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/handle.py
+-rw-r--r--   0 runner     (501) staff       (20)     3136 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/ipython_support.py
+-rw-r--r--   0 runner     (501) staff       (20)    10443 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/log.py
+-rw-r--r--   0 runner     (501) staff       (20)     1853 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/memdebug.py
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/outcomes.py
+-rw-r--r--   0 runner     (501) staff       (20)     5159 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/queue.py
+-rw-r--r--   0 runner     (501) staff       (20)    32968 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/regression.py
+-rw-r--r--   0 runner     (501) staff       (20)     6696 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/result.py
+-rw-r--r--   0 runner     (501) staff       (20)    35588 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    40942 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/scheduler.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.437707 cocotb-1.8.0rc1/cocotb/share/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.476083 cocotb-1.8.0rc1/cocotb/share/def/
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      930 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/aldec.def
+-rw-r--r--   0 runner     (501) staff       (20)      662 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/ghdl.def
+-rw-r--r--   0 runner     (501) staff       (20)      655 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/icarus.def
+-rw-r--r--   0 runner     (501) staff       (20)     2252 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/modelsim.def
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.481112 cocotb-1.8.0rc1/cocotb/share/include/
+-rw-r--r--   0 runner     (501) staff       (20)     3998 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/cocotb_utils.h
+-rw-r--r--   0 runner     (501) staff       (20)     2453 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)      657 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/exports.h
+-rw-r--r--   0 runner     (501) staff       (20)     9999 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/gpi.h
+-rw-r--r--   0 runner     (501) staff       (20)    10341 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/gpi_logging.h
+-rw-r--r--   0 runner     (501) staff       (20)      642 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/py_gpi_logging.h
+-rw-r--r--   0 runner     (501) staff       (20)      628 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/vhpi_user_ext.h
+-rw-r--r--   0 runner     (501) staff       (20)     2456 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/vpi_user_ext.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.437423 cocotb-1.8.0rc1/cocotb/share/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.482299 cocotb-1.8.0rc1/cocotb/share/lib/embed/
+-rw-r--r--   0 runner     (501) staff       (20)     4377 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/embed/embed.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10476 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/embed/gpi_embed.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.485218 cocotb-1.8.0rc1/cocotb/share/lib/fli/
+-rw-r--r--   0 runner     (501) staff       (20)     7754 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    40118 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    16198 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    26850 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliObjHdl.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.487247 cocotb-1.8.0rc1/cocotb/share/lib/gpi/
+-rw-r--r--   0 runner     (501) staff       (20)     4362 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    19643 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCommon.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    11255 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi/gpi_priv.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.487877 cocotb-1.8.0rc1/cocotb/share/lib/gpi_log/
+-rw-r--r--   0 runner     (501) staff       (20)     7056 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi_log/gpi_logging.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.488488 cocotb-1.8.0rc1/cocotb/share/lib/py_gpi_log/
+-rw-r--r--   0 runner     (501) staff       (20)     7022 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.489217 cocotb-1.8.0rc1/cocotb/share/lib/simulator/
+-rw-r--r--   0 runner     (501) staff       (20)    41165 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/simulator/simulatormodule.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.489950 cocotb-1.8.0rc1/cocotb/share/lib/utils/
+-rw-r--r--   0 runner     (501) staff       (20)     3896 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/utils/cocotb_utils.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.490639 cocotb-1.8.0rc1/cocotb/share/lib/verilator/
+-rw-r--r--   0 runner     (501) staff       (20)     4407 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/verilator/verilator.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.492853 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/
+-rw-r--r--   0 runner     (501) staff       (20)    38860 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    36640 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10762 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.495007 cocotb-1.8.0rc1/cocotb/share/lib/vpi/
+-rw-r--r--   0 runner     (501) staff       (20)    27347 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    22748 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10441 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.496844 cocotb-1.8.0rc1/cocotb/share/makefiles/
+-rw-r--r--   0 runner     (501) staff       (20)      416 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.deprecations
+-rw-r--r--   0 runner     (501) staff       (20)     7030 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.inc
+-rw-r--r--   0 runner     (501) staff       (20)     5299 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.sim
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.503902 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/
+-rw-r--r--   0 runner     (501) staff       (20)     2656 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.activehdl
+-rw-r--r--   0 runner     (501) staff       (20)     3901 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.cvc
+-rw-r--r--   0 runner     (501) staff       (20)     3542 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ghdl
+-rw-r--r--   0 runner     (501) staff       (20)     4374 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.icarus
+-rw-r--r--   0 runner     (501) staff       (20)     4965 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ius
+-rw-r--r--   0 runner     (501) staff       (20)     1906 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.modelsim
+-rw-r--r--   0 runner     (501) staff       (20)     6427 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.questa
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.riviera
+-rw-r--r--   0 runner     (501) staff       (20)     3690 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.vcs
+-rw-r--r--   0 runner     (501) staff       (20)     2407 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.verilator
+-rw-r--r--   0 runner     (501) staff       (20)     5414 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.xcelium
+-rw-r--r--   0 runner     (501) staff       (20)    11035 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/task.py
+-rw-r--r--   0 runner     (501) staff       (20)    32228 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/triggers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.507084 cocotb-1.8.0rc1/cocotb/types/
+-rw-r--r--   0 runner     (501) staff       (20)     1803 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10899 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/array.py
+-rw-r--r--   0 runner     (501) staff       (20)     8499 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/logic.py
+-rw-r--r--   0 runner     (501) staff       (20)     9957 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/logic_array.py
+-rw-r--r--   0 runner     (501) staff       (20)     6230 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/range.py
+-rw-r--r--   0 runner     (501) staff       (20)    23064 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     5988 2023-06-12 21:15:21.000000 cocotb-1.8.0rc1/cocotb/wavedrom.py
+-rw-r--r--   0 runner     (501) staff       (20)     3552 2023-06-12 21:15:21.000000 cocotb-1.8.0rc1/cocotb/xunit_reporter.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.462964 cocotb-1.8.0rc1/cocotb.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     6717 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3103 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       53 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)       33 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)      516 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/top_level.txt
+-rwxr-xr-x   0 runner     (501) staff       (20)    27213 2023-06-12 21:15:21.000000 cocotb-1.8.0rc1/cocotb_build_libs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.508117 cocotb-1.8.0rc1/pygpi/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/pygpi/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      946 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/pygpi/entry.py
+-rw-r--r--   0 runner     (501) staff       (20)     2089 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      808 2023-06-12 21:37:16.509804 cocotb-1.8.0rc1/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)     5543 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/setup.py
```

### Comparing `cocotb-1.7.2/LICENSE` & `cocotb-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/PKG-INFO` & `cocotb-1.8.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotb
-Version: 1.7.2
+Version: 1.8.0rc1
 Summary: cocotb is a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 Home-page: https://www.cocotb.org
 Author: Chris Higgs, Stuart Hodgson
 Maintainer: cocotb contributors
 Maintainer-email: cocotb@lists.librecores.org
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cocotb/cocotb/issues
@@ -33,16 +33,15 @@
 [![PyPI](https://img.shields.io/pypi/dm/cocotb.svg?label=PyPI%20downloads)](https://pypi.org/project/cocotb/)
 [![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/cocotb/cocotb)
 [![codecov](https://codecov.io/gh/cocotb/cocotb/branch/master/graph/badge.svg)](https://codecov.io/gh/cocotb/cocotb)
 
 * Read the [documentation](https://docs.cocotb.org)
 * Get involved:
   * [Raise a bug / request an enhancement](https://github.com/cocotb/cocotb/issues/new) (Requires a GitHub account)
-  * [Join the mailing list](https://lists.librecores.org/listinfo/cocotb)
-  * [Join the Gitter chat room](https://gitter.im/cocotb)
+  * [Join the Gitter chat room](https://gitter.im/cocotb/Lobby)
 
 ## Installation
 
 The current stable version of cocotb requires:
 
 - Python 3.6+
 - GNU Make 3+
@@ -92,30 +91,46 @@
 
 An example of a simple randomized cocotb testbench:
 
 ```python
 # test_dff.py
 
 import random
+
 import cocotb
 from cocotb.clock import Clock
-from cocotb.triggers import FallingEdge
+from cocotb.triggers import RisingEdge
+from cocotb.types import LogicArray
 
 @cocotb.test()
-async def test_dff_simple(dut):
-    """ Test that d propagates to q """
+async def dff_simple_test(dut):
+    """Test that d propagates to q"""
+
+    # Assert initial output is unknown
+    assert LogicArray(dut.q.value) == LogicArray("X")
+    # Set initial input value to prevent it from floating
+    dut.d.value = 0
 
     clock = Clock(dut.clk, 10, units="us")  # Create a 10us period clock on port clk
-    cocotb.start_soon(clock.start())  # Start the clock
+    # Start the clock. Start it low to avoid issues on the first RisingEdge
+    cocotb.start_soon(clock.start(start_high=False))
 
+    # Synchronize with the clock. This will regisiter the initial `d` value
+    await RisingEdge(dut.clk)
+    expected_val = 0  # Matches initial input value
     for i in range(10):
         val = random.randint(0, 1)
         dut.d.value = val  # Assign the random value val to the input port d
-        await FallingEdge(dut.clk)
-        assert dut.q.value == val, "output q was incorrect on the {}th cycle".format(i)
+        await RisingEdge(dut.clk)
+        assert dut.q.value == expected_val, f"output q was incorrect on the {i}th cycle"
+        expected_val = val # Save random value for next RisingEdge
+
+    # Check the final input on the next clock
+    await RisingEdge(dut.clk)
+    assert dut.q.value == expected_val, "output q was incorrect on the last cycle"
 ```
 
 A simple Makefile:
 
 ```make
 # Makefile
```

### Comparing `cocotb-1.7.2/README.md` & `cocotb-1.8.0rc1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 [![PyPI](https://img.shields.io/pypi/dm/cocotb.svg?label=PyPI%20downloads)](https://pypi.org/project/cocotb/)
 [![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/cocotb/cocotb)
 [![codecov](https://codecov.io/gh/cocotb/cocotb/branch/master/graph/badge.svg)](https://codecov.io/gh/cocotb/cocotb)
 
 * Read the [documentation](https://docs.cocotb.org)
 * Get involved:
   * [Raise a bug / request an enhancement](https://github.com/cocotb/cocotb/issues/new) (Requires a GitHub account)
-  * [Join the mailing list](https://lists.librecores.org/listinfo/cocotb)
-  * [Join the Gitter chat room](https://gitter.im/cocotb)
+  * [Join the Gitter chat room](https://gitter.im/cocotb/Lobby)
 
 ## Installation
 
 The current stable version of cocotb requires:
 
 - Python 3.6+
 - GNU Make 3+
@@ -64,30 +63,46 @@
 
 An example of a simple randomized cocotb testbench:
 
 ```python
 # test_dff.py
 
 import random
+
 import cocotb
 from cocotb.clock import Clock
-from cocotb.triggers import FallingEdge
+from cocotb.triggers import RisingEdge
+from cocotb.types import LogicArray
 
 @cocotb.test()
-async def test_dff_simple(dut):
-    """ Test that d propagates to q """
+async def dff_simple_test(dut):
+    """Test that d propagates to q"""
+
+    # Assert initial output is unknown
+    assert LogicArray(dut.q.value) == LogicArray("X")
+    # Set initial input value to prevent it from floating
+    dut.d.value = 0
 
     clock = Clock(dut.clk, 10, units="us")  # Create a 10us period clock on port clk
-    cocotb.start_soon(clock.start())  # Start the clock
+    # Start the clock. Start it low to avoid issues on the first RisingEdge
+    cocotb.start_soon(clock.start(start_high=False))
 
+    # Synchronize with the clock. This will regisiter the initial `d` value
+    await RisingEdge(dut.clk)
+    expected_val = 0  # Matches initial input value
     for i in range(10):
         val = random.randint(0, 1)
         dut.d.value = val  # Assign the random value val to the input port d
-        await FallingEdge(dut.clk)
-        assert dut.q.value == val, "output q was incorrect on the {}th cycle".format(i)
+        await RisingEdge(dut.clk)
+        assert dut.q.value == expected_val, f"output q was incorrect on the {i}th cycle"
+        expected_val = val # Save random value for next RisingEdge
+
+    # Check the final input on the next clock
+    await RisingEdge(dut.clk)
+    assert dut.q.value == expected_val, "output q was incorrect on the last cycle"
 ```
 
 A simple Makefile:
 
 ```make
 # Makefile
```

### Comparing `cocotb-1.7.2/cocotb/ANSI.py` & `cocotb-1.8.0rc1/cocotb/ANSI.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/__init__.py` & `cocotb-1.8.0rc1/cocotb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,20 +41,20 @@
 from typing import Dict, List, Optional, Union
 
 import cocotb.handle
 from cocotb._deprecation import deprecated
 from cocotb.log import default_config
 from cocotb.regression import RegressionManager
 from cocotb.scheduler import Scheduler
+from cocotb.task import Task
 
 from ._version import __version__
 
 # Things we want in the cocotb namespace
 from cocotb.decorators import (  # isort: skip # noqa: F401
-    Task,
     coroutine,
     external,
     function,
     test,
 )
 from cocotb.log import _filter_from_c, _log_from_c  # isort: skip # noqa: F401
 
@@ -318,34 +318,23 @@
     global scheduler
     scheduler = Scheduler(handle_result=regression_manager._handle_result)
 
     # start Regression Manager
     regression_manager._execute()
 
 
-def _sim_event(level, message):
+def _sim_event(message):
     """Function that can be called externally to signal an event."""
-    # SIM_INFO = 0
-    SIM_TEST_FAIL = 1
-    SIM_FAIL = 2
     from cocotb.result import SimFailure
 
-    if level is SIM_TEST_FAIL:
-        scheduler.log.error("Failing test at simulator request")
-        scheduler._finish_test(
-            AssertionError(f"Failure from external source: {message}")
-        )
-    elif level is SIM_FAIL:
-        # We simply return here as the simulator will exit
-        # so no cleanup is needed
-        msg = f"Failing test at simulator request before test run completion: {message}"
-        scheduler.log.error(msg)
-        scheduler._finish_scheduler(SimFailure(msg))
-    else:
-        scheduler.log.error("Unsupported sim event")
+    # We simply return here as the simulator will exit
+    # so no cleanup is needed
+    msg = f"Failing test at simulator request before test run completion: {message}"
+    scheduler.log.error(msg)
+    scheduler._finish_scheduler(SimFailure(msg))
 
 
 @deprecated("This function is now private")
 def process_plusargs() -> None:
 
     _process_plusargs()
```

### Comparing `cocotb-1.7.2/cocotb/_deprecation.py` & `cocotb-1.8.0rc1/cocotb/_deprecation.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_py_compat.py` & `cocotb-1.8.0rc1/cocotb/_py_compat.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/README.md` & `cocotb-1.8.0rc1/cocotb/_vendor/README.md`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/distutils_version.py` & `cocotb-1.8.0rc1/cocotb/_vendor/distutils_version.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/fli/acc_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/fli/acc_vhdl.h` & `cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_vhdl.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/fli/mti.h` & `cocotb-1.8.0rc1/cocotb/_vendor/fli/mti.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/tcl/license.terms` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/license.terms`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/tcl/tcl.h` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/tcl.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/tcl/tclDecls.h` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclDecls.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/tcl/tclPlatDecls.h` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclPlatDecls.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/vhpi/vhpi_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/vhpi/vhpi_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/vpi/sv_vpi_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/vpi/sv_vpi_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/_vendor/vpi/vpi_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/vpi/vpi_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/binary.py` & `cocotb-1.8.0rc1/cocotb/binary.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/clock.py` & `cocotb-1.8.0rc1/cocotb/clock.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """A clock class."""
 
 import itertools
 import warnings
+from decimal import Decimal
+from numbers import Real
+from typing import Union
 
 from cocotb.log import SimLog
 from cocotb.triggers import Timer
 from cocotb.utils import get_sim_steps, get_time_from_sim_steps, lazy_property
 
 
 class BaseClock:
@@ -110,26 +113,28 @@
     .. versionchanged:: 1.5
         Support ``'step'`` as the *units* argument to mean "simulator time step".
 
     .. deprecated:: 1.5
         Using ``None`` as the *units* argument is deprecated, use ``'step'`` instead.
     """
 
-    def __init__(self, signal, period, units="step"):
+    def __init__(
+        self, signal, period: Union[float, Real, Decimal], units: str = "step"
+    ):
         BaseClock.__init__(self, signal)
         if units is None:
             warnings.warn(
                 'Using units=None is deprecated, use units="step" instead.',
                 DeprecationWarning,
                 stacklevel=2,
             )
             units = "step"  # don't propagate deprecated value
         self.period = get_sim_steps(period, units)
-        self.half_period = get_sim_steps(period / 2.0, units)
-        self.frequency = 1.0 / get_time_from_sim_steps(self.period, units="us")
+        self.half_period = get_sim_steps(period / 2, units)
+        self.frequency = 1 / get_time_from_sim_steps(self.period, units="us")
         self.hdl = None
         self.signal = signal
         self.coro = None
         self.mcoro = None
 
     async def start(self, cycles=None, start_high=True):
         r"""Clocking coroutine.  Start driving your clock by :func:`cocotb.start`\ ing a
```

### Comparing `cocotb-1.7.2/cocotb/config.py` & `cocotb-1.8.0rc1/cocotb/config.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/handle.py` & `cocotb-1.8.0rc1/cocotb/handle.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/ipython_support.py` & `cocotb-1.8.0rc1/cocotb/ipython_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     default_ns = dict(cocotb=cocotb)
     default_ns.update(user_ns)
 
     # build the config to enable `await`
     c = load_default_config()
     c.TerminalInteractiveShell.loop_runner = lambda x: _runner(shell, x)
     c.TerminalInteractiveShell.autoawait = True
-
+    # Python3 checks SQLite DB accesses to ensure process ID matches the one that opened the DB and is not propogated
+    # because we launch IPython in a different process, this will cause unnecessary warnings, so disable the PID check
+    c.HistoryAccessor.connection_options = {"check_same_thread": False}
     # create a shell with access to the dut, and cocotb pre-imported
     shell = IPython.terminal.embed.InteractiveShellEmbed(
         user_ns=default_ns,
         config=c,
     )
 
     # add our custom prompts
```

### Comparing `cocotb-1.7.2/cocotb/log.py` & `cocotb-1.8.0rc1/cocotb/log.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/memdebug.py` & `cocotb-1.8.0rc1/cocotb/memdebug.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/outcomes.py` & `cocotb-1.8.0rc1/cocotb/outcomes.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/queue.py` & `cocotb-1.8.0rc1/cocotb/queue.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/regression.py` & `cocotb-1.8.0rc1/cocotb/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 import os
 import pdb
 import random
 import sys
 import time
 import traceback
 from itertools import product
-from typing import Any, Iterable, Optional, Tuple
+from typing import Any, Iterable, Optional, Tuple, Type
 
 import cocotb
 import cocotb.ANSI as ANSI
 from cocotb import simulator
 from cocotb._deprecation import deprecated
-from cocotb.decorators import Task
 from cocotb.decorators import test as Test
 from cocotb.handle import SimHandle
 from cocotb.log import SimLog
 from cocotb.outcomes import Error, Outcome
 from cocotb.result import SimFailure, TestSuccess
+from cocotb.task import Task
 from cocotb.utils import get_sim_time, remove_traceback_frames, want_color_output
 from cocotb.xunit_reporter import XUnitReporter
 
 _pdb_on_exception = "COCOTB_PDB_ON_EXCEPTION" in os.environ
 
 # Optional support for coverage collection of testbench files
 coverage = None
@@ -74,14 +74,28 @@
     for comp in components[1:]:
         mod = getattr(mod, comp)
     return mod
 
 
 _logger = SimLog(__name__)
 
+_Failed: Type[BaseException]
+try:
+    import pytest
+except ModuleNotFoundError:
+    _Failed = AssertionError
+else:
+    try:
+        with pytest.raises(Exception):
+            pass
+    except BaseException as _raises_e:
+        _Failed = type(_raises_e)
+    else:
+        assert "pytest.raises doesn't raise an exception when it fails"
+
 
 class RegressionManager:
     """Encapsulates all regression capability into a single place"""
 
     def __init__(self, dut: SimHandle, tests: Iterable[Test]):
         """
         Args:
@@ -246,19 +260,16 @@
             return
         try:
             # Install the assertion rewriting hook, which must be done before we
             # import the test modules.
             from _pytest.assertion import install_importhook
             from _pytest.config import Config
 
-            # Pass python_files to Config to support assertion rewriting only on test modules.
-            # See https://github.com/pytest-dev/pytest/discussions/10052.
-            test_modules_str = " ".join(f"{name}.py" for name in test_modules)
             pytest_conf = Config.fromdictargs(
-                {}, ["--capture=no", "-o", f"python_files={test_modules_str}"]
+                {}, ["--capture=no", "-o", "python_files=*.py"]
             )
             install_importhook(pytest_conf)
         except Exception:
             _logger.exception(
                 "Configuring the assertion rewrite hook using pytest {} failed. "
                 "Please file a bug report!".format(pytest.__version__)
             )
@@ -390,29 +401,28 @@
 
         # scoring outcomes
         result_pass = True
         sim_failed = False
 
         try:
             outcome.get()
-        except Exception as e:
+        except (KeyboardInterrupt, SystemExit):
+            raise
+        except BaseException as e:
             result = remove_traceback_frames(e, ["_score_test", "get"])
         else:
             result = TestSuccess()
 
         if (
             isinstance(result, TestSuccess)
             and not test.expect_fail
             and not test.expect_error
         ):
             self._log_test_passed(test, None, None)
 
-        elif isinstance(result, AssertionError) and test.expect_fail:
-            self._log_test_passed(test, result, "failed as expected")
-
         elif isinstance(result, TestSuccess) and test.expect_error:
             self._log_test_failed(test, None, "passed but we expected an error")
             result_pass = False
 
         elif isinstance(result, TestSuccess):
             self._log_test_failed(test, None, "passed but we expected a failure")
             result_pass = False
@@ -422,14 +432,17 @@
                 self._log_test_passed(test, result, "errored as expected")
             else:
                 self.log.error("Test error has lead to simulator shutting us down")
                 result_pass = False
             # whether we expected it or not, the simulation has failed unrecoverably
             sim_failed = True
 
+        elif isinstance(result, (AssertionError, _Failed)) and test.expect_fail:
+            self._log_test_passed(test, result, "failed as expected")
+
         elif test.expect_error:
             if isinstance(result, test.expect_error):
                 self._log_test_passed(test, result, "errored as expected")
             else:
                 self._log_test_failed(test, result, "errored with unexpected type ")
                 result_pass = False
 
@@ -451,27 +464,30 @@
             rest = ""
         else:
             rest = f": {msg}"
         if result is None:
             result_was = ""
         else:
             result_was = f" (result was {type(result).__qualname__})"
-        self.log.info(f"{test} {start_hilight}passed{stop_hilight}{rest}{result_was}")
+        self.log.info(
+            f"{test.__qualname__} {start_hilight}passed{stop_hilight}{rest}{result_was}"
+        )
 
     def _log_test_failed(
         self, test: Test, result: Optional[Exception] = None, msg: Optional[str] = None
     ) -> None:
         start_hilight = ANSI.COLOR_FAILED if want_color_output() else ""
         stop_hilight = ANSI.COLOR_DEFAULT if want_color_output() else ""
         if msg is None:
             rest = ""
         else:
             rest = f": {msg}"
         self.log.info(
-            f"{test} {start_hilight}failed{stop_hilight}{rest}", exc_info=result
+            f"{test.__qualname__} {start_hilight}failed{stop_hilight}{rest}",
+            exc_info=result,
         )
 
     def _record_result(
         self,
         test: Test,
         outcome: Optional[Outcome],
         wall_time_s: float,
@@ -498,15 +514,17 @@
             test_pass, sim_failed = None, False
             self.xunit.add_skipped()
             self.skipped += 1
 
         else:
             test_pass, sim_failed = self._score_test(test, outcome)
             if not test_pass:
-                self.xunit.add_failure()
+                self.xunit.add_failure(
+                    message=f"Test failed with RANDOM_SEED={cocotb.RANDOM_SEED}"
+                )
                 self.failures += 1
             else:
                 self.passed += 1
 
         self.test_results.append(
             {
                 "test": ".".join([test.__module__, test.__qualname__]),
@@ -888,15 +906,15 @@
 
 
 def _trim(docstring: Optional[str]) -> str:
     """Normalizes test docstrings
 
     Based on https://www.python.org/dev/peps/pep-0257/#handling-docstring-indentation.
     """
-    if docstring is None:
+    if docstring is None or docstring == "":
         return ""
     # Convert tabs to spaces (following the normal Python rules)
     # and split into a list of lines:
     lines = docstring.expandtabs().splitlines()
     # Determine minimum indentation (first line doesn't count):
     indent = math.inf
     for line in lines[1:]:
```

### Comparing `cocotb-1.7.2/cocotb/result.py` & `cocotb-1.8.0rc1/cocotb/result.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/runner.py` & `cocotb-1.8.0rc1/cocotb/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 # Copyright cocotb contributors
 # Licensed under the Revised BSD License, see LICENSE for details.
 # SPDX-License-Identifier: BSD-3-Clause
 
+"""Build HDL and run cocotb tests."""
+
+# TODO: maybe do globbing and expanduser/expandvars in --include, --vhdl-sources, --verilog-sources
+# TODO: create a short README and a .gitignore (content: "*") in both build_dir and test_dir? (Some other tools do this.)
+# TODO: support timescale
+# TODO: support custom dependencies
+
 import abc
 import os
 import re
+import shlex
 import shutil
 import subprocess
 import sys
 import tempfile
 import warnings
 from contextlib import suppress
-from typing import Dict, List, Mapping, Optional, Sequence, Type, Union
+from pathlib import Path
+from typing import Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
 from xml.etree import cElementTree as ET
 
 import find_libpython
 
 import cocotb.config
 
 PathLike = Union["os.PathLike[str]", str]
@@ -38,672 +47,744 @@
     value = _space_re.sub(r"\\\1", value)
     if value[0] == '"':
         value = "\\" + value
 
     return value
 
 
+def shlex_join(split_command):
+    """
+    Return a shell-escaped string from *split_command*
+    This is here more for compatibility purposes
+    """
+    return " ".join(shlex.quote(arg) for arg in split_command)
+
+
 class Simulator(abc.ABC):
+
+    supported_gpi_interfaces: Dict[str, List[str]] = {}
+
     def __init__(self) -> None:
 
-        self.simulator_in_path()
+        self._simulator_in_path()
 
         self.env: Dict[str, str] = {}
 
         # for running test() independently of build()
-        self.build_dir = "sim_build"
-        self.parameters = {}
+        self.build_dir: Path = get_abs_path("sim_build")
+        self.parameters: Mapping[str, object] = {}
 
     @abc.abstractmethod
-    def simulator_in_path(self) -> None:
-        """Check that the simulator executable exists in :envvar:`PATH`."""
+    def _simulator_in_path(self) -> None:
+        """Raise exception if the simulator executable does not exist in :envvar:`PATH`.
+
+        Raises:
+            SystemExit: Simulator executable does not exist in :envvar:`PATH`.
+        """
 
         raise NotImplementedError()
 
-    @abc.abstractmethod
-    def check_toplevel_lang(self, toplevel_lang: Optional[str]) -> str:
-        """Return *toplevel_lang* if supported by simulator, raise exception otherwise."""
+    def _check_hdl_toplevel_lang(self, hdl_toplevel_lang: Optional[str]) -> str:
+        """Return *hdl_toplevel_lang* if supported by simulator, raise exception otherwise.
 
-        raise NotImplementedError()
+        Returns:
+            *hdl_toplevel_lang* if supported by the simulator.
 
-    def set_env(self) -> None:
+        Raises:
+            ValueError: *hdl_toplevel_lang* is not supported by the simulator.
+        """
+        if hdl_toplevel_lang is None:
+            if self.vhdl_sources and not self.verilog_sources:
+                lang = "vhdl"
+            elif self.verilog_sources and not self.vhdl_sources:
+                lang = "verilog"
+            else:
+                raise ValueError(
+                    f"{type(self).__qualname__}: Must specify a hdl_toplevel_lang in a mixed-language design"
+                )
+        else:
+            lang = hdl_toplevel_lang
+
+        if lang in self.supported_gpi_interfaces.keys():
+            return lang
+        else:
+            raise ValueError(
+                f"{type(self).__qualname__}: hdl_toplevel_lang {hdl_toplevel_lang!r} is not "
+                f"in supported list: {', '.join(self.supported_gpi_interfaces.keys())}"
+            )
+
+    def _set_env(self) -> None:
         """Set environment variables for sub-processes."""
 
         for e in os.environ:
             self.env[e] = os.environ[e]
 
         if "LIBPYTHON_LOC" not in self.env:
             self.env["LIBPYTHON_LOC"] = find_libpython.find_libpython()
 
         self.env["PATH"] += os.pathsep + cocotb.config.libs_dir
-
         self.env["PYTHONPATH"] = os.pathsep.join(sys.path)
-        for path in self.python_search:
-            self.env["PYTHONPATH"] += os.pathsep + str(path)
-
         self.env["PYTHONHOME"] = sys.prefix
-
-        self.env["TOPLEVEL"] = self.sim_toplevel
-        self.env["MODULE"] = self.module
+        self.env["TOPLEVEL"] = self.sim_hdl_toplevel
+        self.env["MODULE"] = self.test_module
 
     @abc.abstractmethod
-    def build_command(self) -> Sequence[Command]:
+    def _build_command(self) -> Sequence[Command]:
         """Return command to build the HDL sources."""
 
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def test_command(self) -> Sequence[Command]:
+    def _test_command(self) -> Sequence[Command]:
         """Return command to run a test."""
 
         raise NotImplementedError()
 
     def build(
         self,
-        library_name: str = "work",
+        hdl_library: str = "top",
         verilog_sources: Sequence[PathLike] = [],
         vhdl_sources: Sequence[PathLike] = [],
         includes: Sequence[PathLike] = [],
-        defines: Sequence[str] = [],
+        defines: Mapping[str, object] = {},
         parameters: Mapping[str, object] = {},
-        extra_args: Sequence[str] = [],
-        toplevel: Optional[str] = None,
+        build_args: Sequence[str] = [],
+        hdl_toplevel: Optional[str] = None,
         always: bool = False,
         build_dir: PathLike = "sim_build",
+        verbose: bool = False,
     ) -> None:
-        """Build the HDL sources."""
+        """Build the HDL sources.
+
+        Args:
+            hdl_library: The library name to compile into.
+            verilog_sources: Verilog source files to build.
+            vhdl_sources: VHDL source files to build.
+            includes: Verilog include directories.
+            defines: Defines to set.
+            parameters: Verilog parameters or VHDL generics.
+            build_args: Extra build arguments for the simulator.
+            hdl_toplevel: The name of the HDL toplevel module.
+            always: Always run the build step.
+            build_dir: Directory to run the build step in.
+            verbose: Enable verbose messages.
+        """
 
-        self.build_dir = os.path.abspath(build_dir)
+        self.build_dir = get_abs_path(build_dir)
         os.makedirs(self.build_dir, exist_ok=True)
 
         # note: to avoid mutating argument defaults, we ensure that no value
         # is written without a copy. This is much more concise and leads to
         # a better docstring than using `None` as a default in the parameters
         # list.
-        self.library_name = library_name
-        self.verilog_sources = get_abs_paths(verilog_sources)
-        self.vhdl_sources = get_abs_paths(vhdl_sources)
-        self.includes = get_abs_paths(includes)
-        self.defines = list(defines)
+        self.hdl_library: str = hdl_library
+        self.verilog_sources: List[Path] = get_abs_paths(verilog_sources)
+        self.vhdl_sources: List[Path] = get_abs_paths(vhdl_sources)
+        self.includes: List[Path] = get_abs_paths(includes)
+        self.defines = dict(defines)
         self.parameters = dict(parameters)
-        self.compile_args = list(extra_args)
-        self.always = always
-        self.hdl_toplevel = toplevel
+        self.build_args = list(build_args)
+        self.always: bool = always
+        self.hdl_toplevel: Optional[str] = hdl_toplevel
+        self.verbose: bool = verbose
 
         for e in os.environ:
             self.env[e] = os.environ[e]
 
-        cmds = self.build_command()
-        self.execute(cmds, cwd=self.build_dir)
+        cmds: Sequence[Command] = self._build_command()
+        self._execute(cmds, cwd=self.build_dir)
 
     def test(
         self,
-        py_module: Union[str, Sequence[str]],
-        toplevel: str,
-        toplevel_lang: Optional[str] = None,
-        testcase: Optional[str] = None,
+        test_module: Union[str, Sequence[str]],
+        hdl_toplevel: str,
+        hdl_toplevel_library: str = "top",
+        hdl_toplevel_lang: Optional[str] = None,
+        gpi_interfaces: Optional[List[str]] = None,
+        testcase: Optional[Union[str, Sequence[str]]] = None,
         seed: Optional[Union[str, int]] = None,
-        python_search: Sequence[PathLike] = [],
-        extra_args: Sequence[str] = [],
-        plus_args: Sequence[str] = [],
+        test_args: Sequence[str] = [],
+        plusargs: Sequence[str] = [],
         extra_env: Mapping[str, str] = {},
         waves: Optional[bool] = None,
         gui: Optional[bool] = None,
         parameters: Mapping[str, object] = None,
         build_dir: Optional[PathLike] = None,
-        sim_dir: Optional[PathLike] = None,
-    ) -> PathLike:
-        """Run a test."""
+        test_dir: Optional[PathLike] = None,
+        results_xml: str = "results.xml",
+        verbose: bool = False,
+    ) -> Path:
+        """Run the tests.
+
+        Args:
+            test_module: Name(s) of the Python module(s) containing the tests to run.
+                Can be a comma-separated list.
+            hdl_toplevel: Name of the HDL toplevel module.
+            hdl_toplevel_library: The library name for HDL toplevel module.
+            hdl_toplevel_lang: Language of the HDL toplevel module.
+            gpi_interfaces: List of GPI interfaces to use, with the first one being the entry point.
+            testcase: Name(s) of a specific testcase(s) to run.
+                If not set, run all testcases found in *test_module*.
+                Can be a comma-separated list.
+            seed: A specific random seed to use.
+            test_args: Extra arguments for the simulator.
+            plusargs: 'plusargs' to set for the simulator.
+            extra_env: Extra environment variables to set.
+            waves: Record signal traces.
+            gui: Run with simulator GUI.
+            parameters: Verilog parameters or VHDL generics.
+            build_dir: Directory the build step has been run in.
+            test_dir: Directory to run the tests in.
+            results_xml: Name of xUnit XML file to store test results in.
+                When running with pytest, the testcase name is prefixed to this name.
+            verbose: Enable verbose messages.
+
+        Returns:
+            The absolute location of the results XML file which can be
+            defined by the *results_xml* argument.
+            The default is :file:`{build_dir}/{pytest_test_name}.results.xml`
+            when run with ``pytest``,
+            :file:`{build_dir}/results.xml` otherwise.
+        """
 
         __tracebackhide__ = True  # Hide the traceback when using pytest
 
         if build_dir is not None:
-            self.build_dir = build_dir
+            self.build_dir = get_abs_path(build_dir)
 
         if parameters is not None:
             self.parameters = dict(parameters)
 
-        if sim_dir is None:
-            self.sim_dir = self.build_dir
+        if test_dir is None:
+            self.test_dir = self.build_dir
         else:
-            self.sim_dir = os.path.abspath(sim_dir)
+            self.test_dir = get_abs_path(test_dir)
+        os.makedirs(self.test_dir, exist_ok=True)
 
-        if isinstance(py_module, str):
-            self.module = py_module
+        if isinstance(test_module, str):
+            self.test_module = test_module
         else:
-            self.module = ",".join(py_module)
+            self.test_module = ",".join(test_module)
 
         # note: to avoid mutating argument defaults, we ensure that no value
         # is written without a copy. This is much more concise and leads to
         # a better docstring than using `None` as a default in the parameters
         # list.
-        self.python_search = list(python_search)
-        self.sim_toplevel = toplevel
-        self.toplevel_lang = self.check_toplevel_lang(toplevel_lang)
-        self.sim_args = list(extra_args)
-        self.plus_args = list(plus_args)
+        self.sim_hdl_toplevel = hdl_toplevel
+        self.hdl_toplevel_library: str = hdl_toplevel_library
+        self.hdl_toplevel_lang = self._check_hdl_toplevel_lang(hdl_toplevel_lang)
+        if gpi_interfaces:
+            self.gpi_interfaces = gpi_interfaces
+        else:
+            self.gpi_interfaces = []
+            for gpi_if in self.supported_gpi_interfaces.values():
+                self.gpi_interfaces.append(gpi_if[0])
+
+        self.test_args = list(test_args)
+        self.plusargs = list(plusargs)
         self.env = dict(extra_env)
 
         if testcase is not None:
-            self.env["TESTCASE"] = testcase
+            if isinstance(testcase, str):
+                self.env["TESTCASE"] = testcase
+            else:
+                self.env["TESTCASE"] = ",".join(testcase)
 
         if seed is not None:
             self.env["RANDOM_SEED"] = str(seed)
 
-        if waves is None:
-            self.waves = bool(int(os.getenv("COCOTB_WAVES", 0)))
-        else:
-            self.waves = bool(waves)
+        self.waves = bool(waves)
+        self.gui = bool(gui)
 
-        if gui is None:
-            self.gui = bool(int(os.getenv("COCOTB_GUI", 0)))
-        else:
-            self.gui = bool(gui)
+        if verbose is not None:
+            self.verbose = verbose
 
         # When using pytest, use test name as result file name
         pytest_current_test = os.getenv("PYTEST_CURRENT_TEST", "")
         if pytest_current_test:
             self.current_test_name = pytest_current_test.split(":")[-1].split(" ")[0]
-            results_xml_name = f"{self.current_test_name}.results.xml"
+            results_xml_name = f"{self.current_test_name}.{results_xml}"
         else:
             self.current_test_name = "test"
-            results_xml_name = "results.xml"
-
-        results_xml_file = os.getenv(
-            "COCOTB_RESULTS_FILE", os.path.join(self.build_dir, results_xml_name)
-        )
+            results_xml_name = results_xml
 
-        self.env["COCOTB_RESULTS_FILE"] = results_xml_file
+        results_xml_file = Path(self.test_dir) / results_xml_name
 
         with suppress(OSError):
             os.remove(results_xml_file)
 
-        cmds = self.test_command()
-        self.set_env()
-        self.execute(cmds, cwd=self.sim_dir)
-
-        check_results_file(results_xml_file)
+        # transport the settings to cocotb via environment variables
+        self._set_env()
+        self.env["COCOTB_RESULTS_FILE"] = str(results_xml_file)
+
+        cmds: Sequence[Command] = self._test_command()
+        self._execute(cmds, cwd=self.test_dir)
+
+        # Only when running under pytest, check the results file here,
+        # potentially raising an exception with failing testcases,
+        # otherwise return the results file for later analysis.
+        if pytest_current_test:
+            check_results_file(results_xml_file)
 
         print(f"INFO: Results file: {results_xml_file}")
         return results_xml_file
 
-    @abc.abstractmethod
-    def get_include_options(self, includes: Sequence[str]) -> List[str]:
-        """Return simulator options setting directories searched for Verilog include files."""
+    @staticmethod
+    def _get_include_options(self, includes: Sequence[PathLike]) -> Command:
+        """Return simulator-specific formatted option strings with *includes* directories."""
 
         raise NotImplementedError()
 
-    @abc.abstractmethod
-    def get_define_options(self, defines: Sequence[str]) -> List[str]:
-        """Return simulator options defining macros."""
+    @staticmethod
+    def _get_define_options(self, defines: Mapping[str, object]) -> Command:
+        """Return simulator-specific formatted option strings with *defines* macros."""
 
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def get_parameter_options(self, parameters: Mapping[str, object]) -> List[str]:
-        """Return simulator options for module parameters/generics."""
+    def _get_parameter_options(self, parameters: Mapping[str, object]) -> Command:
+        """Return simulator-specific formatted option strings with *parameters*/generics."""
 
         raise NotImplementedError()
 
-    def execute(self, cmds: Sequence[Command], cwd: PathLike) -> None:
+    def _execute(self, cmds: Sequence[Command], cwd: PathLike) -> None:
 
         __tracebackhide__ = True  # Hide the traceback when using PyTest.
 
         for cmd in cmds:
-            print(
-                "INFO: Running command: "
-                + ' "'.join(cmd)
-                + '" in directory:"'
-                + str(cwd)
-                + '"'
-            )
+            print(f"INFO: Running command {shlex_join(cmd)} in directory {cwd}")
 
             # TODO: create a thread to handle stderr and log as error?
             # TODO: log forwarding
 
             process = subprocess.run(cmd, cwd=cwd, env=self.env)
 
             if process.returncode != 0:
                 raise SystemExit(
                     f"Process {process.args[0]!r} terminated with error {process.returncode}"
                 )
 
 
-def check_results_file(results_xml_file: PathLike) -> None:
-    """Check whether cocotb result file exists and contains failed tests."""
+def get_results(results_xml_file: Path) -> Tuple[int, int]:
+    """Return number of tests and fails in *results_xml_file*.
+
+    Returns:
+        Tuple of number of tests and number of fails.
+
+    Raises:
+        SystemExit: *results_xml_file* is non-existent.
+    """
 
     __tracebackhide__ = True  # Hide the traceback when using PyTest.
 
-    results_file_exist = os.path.isfile(results_xml_file)
-    if not results_file_exist:
+    if not results_xml_file.is_file():
         raise SystemExit(
-            "ERROR: Simulation terminated abnormally. Results file not found."
+            f"ERROR: Simulation terminated abnormally. Results file {results_xml_file} not found."
         )
 
-    failed = 0
+    num_tests = 0
+    num_failed = 0
 
     tree = ET.parse(results_xml_file)
     for ts in tree.iter("testsuite"):
         for tc in ts.iter("testcase"):
+            num_tests += 1
             for _ in tc.iter("failure"):
-                failed += 1
+                num_failed += 1
+
+    return (num_tests, num_failed)
+
+
+def check_results_file(results_xml_file: Path) -> None:
+    """Raise exception if *results_xml_file* does not exist or contains failed tests.
+
+    Raises:
+        SystemExit: *results_xml_file* is non-existent or contains fails.
+    """
+
+    __tracebackhide__ = True  # Hide the traceback when using PyTest.
 
-    if failed:
-        raise SystemExit(f"ERROR: Failed {failed} tests.")
+    (num_tests, num_failed) = get_results(results_xml_file)
 
+    if num_failed:
+        raise SystemExit(f"ERROR: Failed {num_failed} of {num_tests} tests.")
 
-def outdated(output: PathLike, dependencies: Sequence[PathLike]) -> bool:
-    """Check if source files are newer than output."""
 
-    if not os.path.isfile(output):
+def outdated(output: Path, dependencies: Sequence[Path]) -> bool:
+    """Return ``True`` if any source files in *dependencies* are newer than the *output* directory.
+
+    Returns:
+        ``True`` if any source files are newer, ``False`` otherwise.
+    """
+
+    if not output.is_file():
         return True
 
-    output_mtime = os.path.getmtime(output)
+    output_mtime = output.stat().st_mtime
 
     dep_mtime = 0.0
-    for file in dependencies:
-        mtime = os.path.getmtime(file)
+    for dependency in dependencies:
+        mtime = dependency.stat().st_mtime
         if mtime > dep_mtime:
             dep_mtime = mtime
 
-    if dep_mtime > output_mtime:
-        return True
+    return dep_mtime > output_mtime
 
-    return False
 
+def get_abs_path(path: PathLike) -> Path:
+    """Return *path* in absolute form."""
 
-def get_abs_paths(paths: Sequence[PathLike]) -> List[str]:
-    """Return list of *paths* in absolute form."""
+    path = Path(path)
+    if path.is_absolute():
+        return path.resolve()
+    else:
+        return Path(Path.cwd() / path).resolve()
 
-    paths_abs: List[str] = []
-    for path in paths:
-        if os.path.isabs(path):
-            paths_abs.append(os.path.abspath(path))
-        else:
-            paths_abs.append(os.path.abspath(os.path.join(os.getcwd(), path)))
 
-    return paths_abs
+def get_abs_paths(paths: Sequence[PathLike]) -> List[Path]:
+    """Return list of *paths* in absolute form."""
+
+    return [get_abs_path(path) for path in paths]
 
 
 class Icarus(Simulator):
-    @staticmethod
-    def simulator_in_path() -> None:
-        if shutil.which("iverilog") is None:
-            raise SystemExit("ERROR: iverilog exacutable not found!")
+    supported_gpi_interfaces = {"verilog": ["vpi"]}
 
     @staticmethod
-    def check_toplevel_lang(toplevel_lang: Optional[str]) -> str:
-        if toplevel_lang is None or toplevel_lang == "verilog":
-            return "verilog"
-        else:
-            raise ValueError(
-                f"iverilog does not support {toplevel_lang!r} as a toplevel_lang"
-            )
+    def _simulator_in_path() -> None:
+        if shutil.which("iverilog") is None:
+            raise SystemExit("ERROR: iverilog executable not found!")
 
     @staticmethod
-    def get_include_options(includes: Sequence[str]) -> List[str]:
-        return ["-I" + dir for dir in includes]
+    def _get_include_options(includes: Sequence[PathLike]) -> Command:
+        return [f"-I{include}" for include in includes]
 
     @staticmethod
-    def get_define_options(defines: Sequence[str]) -> List[str]:
-        return ["-D" + define for define in defines]
+    def _get_define_options(defines: Mapping[str, object]) -> Command:
+        return [f"-D{name}={value}" for name, value in defines.items()]
 
-    def get_parameter_options(self, parameters: Mapping[str, object]) -> List[str]:
+    def _get_parameter_options(self, parameters: Mapping[str, object]) -> Command:
         assert self.hdl_toplevel is not None
         return [
             f"-P{self.hdl_toplevel}.{name}={value}"
             for name, value in parameters.items()
         ]
 
     @property
-    def sim_file(self) -> PathLike:
-        return os.path.join(self.build_dir, "sim.vvp")
+    def sim_file(self) -> Path:
+        return self.build_dir / "sim.vvp"
 
-    def test_command(self) -> List[Command]:
+    def _test_command(self) -> List[Command]:
 
         return [
             [
                 "vvp",
                 "-M",
                 cocotb.config.libs_dir,
                 "-m",
                 cocotb.config.lib_name("vpi", "icarus"),
             ]
-            + self.sim_args
-            + [self.sim_file]
-            + self.plus_args
+            + self.test_args
+            + [str(self.sim_file)]
+            + self.plusargs
         ]
 
-    def build_command(self) -> List[Command]:
+    def _build_command(self) -> List[Command]:
 
         if self.vhdl_sources:
-            raise ValueError("This simulator does not support VHDL")
+            raise ValueError(
+                f"{type(self).__qualname__}: Simulator does not support VHDL"
+            )
 
-        cmd = []
+        cmds = []
         if outdated(self.sim_file, self.verilog_sources) or self.always:
 
-            cmd = [
-                ["iverilog", "-o", self.sim_file, "-D", "COCOTB_SIM=1", "-g2012"]
-                + self.get_define_options(self.defines)
-                + self.get_include_options(self.includes)
-                + self.get_parameter_options(self.parameters)
-                + self.compile_args
-                + self.verilog_sources
+            cmds = [
+                ["iverilog", "-o", str(self.sim_file), "-D", "COCOTB_SIM=1", "-g2012"]
+                + self._get_define_options(self.defines)
+                + self._get_include_options(self.includes)
+                + self._get_parameter_options(self.parameters)
+                + self.build_args
+                + [str(source_file) for source_file in self.verilog_sources]
             ]
 
         else:
-            print("WARNING: Skipping compilation:" + self.sim_file)
+            print("WARNING: Skipping compilation of", self.sim_file)
 
-        return cmd
+        return cmds
 
 
 class Questa(Simulator):
+    supported_gpi_interfaces = {"verilog": ["vpi"], "vhdl": ["fli", "vhpi"]}
+
     @staticmethod
-    def simulator_in_path() -> None:
+    def _simulator_in_path() -> None:
         if shutil.which("vsim") is None:
             raise SystemExit("ERROR: vsim executable not found!")
 
-    def check_toplevel_lang(self, toplevel_lang: Optional[str]) -> str:
-        if toplevel_lang is None:
-            if self.vhdl_sources and not self.verilog_sources:
-                return "vhdl"
-            elif self.verilog_sources and not self.vhdl_sources:
-                return "verilog"
-            else:
-                raise ValueError("Must specify a toplevel_lang in a mixed design")
-        elif toplevel_lang in ("verilog", "vhdl"):
-            return toplevel_lang
-        else:
-            raise ValueError(
-                f"Questa does not support {toplevel_lang!r} as a toplevel_lang"
-            )
-
     @staticmethod
-    def get_include_options(includes: Sequence[str]) -> List[str]:
-        return ["+incdir+" + as_tcl_value(dir) for dir in includes]
+    def _get_include_options(includes: Sequence[PathLike]) -> Command:
+        return [f"+incdir+{as_tcl_value(str(include))}" for include in includes]
 
     @staticmethod
-    def get_define_options(defines: Sequence[str]) -> List[str]:
-        return ["+define+" + as_tcl_value(define) for define in defines]
+    def _get_define_options(defines: Mapping[str, object]) -> Command:
+        return [
+            f"+define+{as_tcl_value(name)}={as_tcl_value(str(value))}"
+            for name, value in defines.items()
+        ]
 
     @staticmethod
-    def get_parameter_options(parameters: Mapping[str, object]) -> List[str]:
-        return ["-g" + name + "=" + str(value) for name, value in parameters.items()]
+    def _get_parameter_options(parameters: Mapping[str, object]) -> Command:
+        return [f"-g{name}={value}" for name, value in parameters.items()]
 
-    def build_command(self) -> List[Command]:
+    def _build_command(self) -> List[Command]:
 
-        cmd = []
+        cmds = []
 
         if self.vhdl_sources:
-            cmd.append(["vlib", as_tcl_value(self.library_name)])
-            cmd.append(
-                ["vcom", "-mixedsvvh"]
-                + ["-work", as_tcl_value(self.library_name)]
-                + [as_tcl_value(v) for v in self.compile_args]
-                + [as_tcl_value(v) for v in self.vhdl_sources]
+            cmds.append(["vlib", as_tcl_value(self.hdl_library)])
+            cmds.append(
+                ["vcom"]
+                + ["-work", as_tcl_value(self.hdl_library)]
+                + [as_tcl_value(v) for v in self.build_args]
+                + [as_tcl_value(str(v)) for v in self.vhdl_sources]
             )
 
         if self.verilog_sources:
-            cmd.append(["vlib", as_tcl_value(self.library_name)])
-            cmd.append(
-                ["vlog", "-mixedsvvh"]
+            cmds.append(["vlib", as_tcl_value(self.hdl_library)])
+            cmds.append(
+                ["vlog"]
                 + ([] if self.always else ["-incr"])
-                + ["-work", as_tcl_value(self.library_name)]
+                + ["-work", as_tcl_value(self.hdl_library)]
                 + ["+define+COCOTB_SIM"]
                 + ["-sv"]
-                + self.get_define_options(self.defines)
-                + self.get_include_options(self.includes)
-                + [as_tcl_value(v) for v in self.compile_args]
-                + [as_tcl_value(v) for v in self.verilog_sources]
+                + self._get_define_options(self.defines)
+                + self._get_include_options(self.includes)
+                + [as_tcl_value(v) for v in self.build_args]
+                + [as_tcl_value(str(v)) for v in self.verilog_sources]
             )
 
-        return cmd
+        return cmds
 
-    def test_command(self) -> List[Command]:
+    def _test_command(self) -> List[Command]:
 
-        cmd = []
+        cmds = []
 
         do_script = ""
         if self.waves:
             do_script += "log -recursive /*;"
 
         if not self.gui:
             do_script += "run -all; quit"
 
-        fli_lib_path = cocotb.config.lib_name_path("fli", "questa")
+        gpi_if_entry = self.gpi_interfaces[0]
+        gpi_if_entry_lib_path = cocotb.config.lib_name_path(gpi_if_entry, "questa")
 
-        if self.toplevel_lang == "vhdl":
-
-            if not os.path.isfile(fli_lib_path):
-                raise SystemExit(
-                    "ERROR: cocotb was not installed with an FLI library, as the mti.h header could not be located.\n\
-                    If you installed an FLI-capable simulator after cocotb, you will need to reinstall cocotb.\n\
-                    Please check the cocotb documentation on ModelSim support."
-                )
+        if gpi_if_entry == "fli":
+            lib_opts = [
+                "-foreign",
+                "cocotb_init "
+                + as_tcl_value(cocotb.config.lib_name_path("fli", "questa")),
+            ]
+        elif gpi_if_entry == "vhpi":
+            lib_opts = ["-voptargs=-access=rw+/."]
+            lib_opts += [
+                "-foreign",
+                "vhpi_startup_routines_bootstrap "
+                + as_tcl_value(cocotb.config.lib_name_path("vhpi", "questa")),
+            ]
+        else:
+            lib_opts = [
+                "-pli",
+                as_tcl_value(cocotb.config.lib_name_path("vpi", "questa")),
+            ]
 
-            cmd.append(
-                ["vsim"]
-                + ["-gui" if self.gui else "-c"]
-                + ["-onfinish", "stop" if self.gui else "exit"]
-                + [
-                    "-foreign",
-                    "cocotb_init "
-                    + as_tcl_value(cocotb.config.lib_name_path("fli", "questa")),
-                ]
-                + [as_tcl_value(v) for v in self.sim_args]
-                + [as_tcl_value(v) for v in self.get_parameter_options(self.parameters)]
-                + [as_tcl_value(self.sim_toplevel)]
-                + ["-do", do_script]
+        if not Path(gpi_if_entry_lib_path).is_file():
+            raise SystemExit(
+                "ERROR: cocotb was not installed with a {gpi_if_entry} library."
             )
 
-            self.env["GPI_EXTRA"] = (
-                cocotb.config.lib_name_path("vpi", "questa") + ":cocotbvpi_entry_point"
-            )
+        cmds.append(
+            ["vsim"]
+            + ["-gui" if self.gui else "-c"]
+            + ["-onfinish", "stop" if self.gui else "exit"]
+            + lib_opts
+            + [as_tcl_value(v) for v in self.test_args]
+            + [as_tcl_value(v) for v in self._get_parameter_options(self.parameters)]
+            + [as_tcl_value(f"{self.hdl_toplevel_library}.{self.sim_hdl_toplevel}")]
+            + [as_tcl_value(v) for v in self.plusargs]
+            + ["-do", do_script]
+        )
 
-        else:
-            cmd.append(
-                ["vsim"]
-                + ["-gui" if self.gui else "-c"]
-                + ["-onfinish", "stop" if self.gui else "exit"]
-                + ["-pli", as_tcl_value(cocotb.config.lib_name_path("vpi", "questa"))]
-                + [as_tcl_value(v) for v in self.sim_args]
-                + [as_tcl_value(v) for v in self.get_parameter_options(self.parameters)]
-                + [as_tcl_value(self.sim_toplevel)]
-                + [as_tcl_value(v) for v in self.plus_args]
-                + ["-do", do_script]
-            )
-
-            if os.path.isfile(fli_lib_path):
-                self.env["GPI_EXTRA"] = (
-                    cocotb.config.lib_name_path("fli", "questa")
-                    + ":cocotbfli_entry_point"
+        gpi_extra_list = []
+        for gpi_if in self.gpi_interfaces[1:]:
+            gpi_if_lib_path = cocotb.config.lib_name_path(gpi_if, "questa")
+            if Path(gpi_if_lib_path).is_file():
+                gpi_extra_list.append(
+                    cocotb.config.lib_name_path(gpi_if, "questa")
+                    + f":cocotb{gpi_if}_entry_point"
                 )
             else:
-                print(
-                    "WARNING: FLI library not found. Mixed-mode simulation will not be available."
-                )
+                print("WARNING: {gpi_if_lib_path} library not found.")
+        self.env["GPI_EXTRA"] = ",".join(gpi_extra_list)
 
-        return cmd
+        return cmds
 
 
 class Ghdl(Simulator):
+    supported_gpi_interfaces = {"vhdl": ["vpi"]}
+
     @staticmethod
-    def simulator_in_path() -> None:
+    def _simulator_in_path() -> None:
         if shutil.which("ghdl") is None:
             raise SystemExit("ERROR: ghdl executable not found!")
 
-    def check_toplevel_lang(self, toplevel_lang: Optional[str]) -> str:
-        if toplevel_lang is None or toplevel_lang == "vhdl":
-            return "vhdl"
-        else:
-            raise ValueError(
-                f"GHDL does not support {toplevel_lang!r} as a toplevel_lang"
-            )
-
-    @staticmethod
-    def get_include_options(includes: Sequence[str]) -> List[str]:
-        return [f"-I{dir}" for dir in includes]
-
-    @staticmethod
-    def get_define_options(defines: Sequence[str]) -> List[str]:
-        return [f"-D{define}" for define in defines]
-
     @staticmethod
-    def get_parameter_options(parameters: Mapping[str, object]) -> List[str]:
-        return ["-g" + name + "=" + str(value) for name, value in parameters.items()]
+    def _get_parameter_options(parameters: Mapping[str, object]) -> Command:
+        return [f"-g{name}={value}" for name, value in parameters.items()]
 
-    def build_command(self) -> List[Command]:
+    def _build_command(self) -> List[Command]:
 
         if self.verilog_sources:
-            raise ValueError("This simulator does not support Verilog")
-
-        if self.hdl_toplevel is None:
             raise ValueError(
-                "This simulator requires the hdl_toplevel parameter to be specified"
+                f"{type(self).__qualname__}: Simulator does not support Verilog"
             )
 
-        cmd = [
+        cmds = [
             ["ghdl", "-i"]
-            + [f"--work={self.library_name}"]
-            + self.compile_args
-            + [source_file]
-            for source_file in self.vhdl_sources
+            + [f"--work={self.hdl_library}"]
+            + self.build_args
+            + [str(source_file) for source_file in self.vhdl_sources]
         ]
 
-        cmd += [
-            ["ghdl", "-m"]
-            + [f"--work={self.library_name}"]
-            + self.compile_args
-            + [self.hdl_toplevel]
-        ]
+        if self.hdl_toplevel is not None:
+            cmds += [
+                ["ghdl", "-m"]
+                + [f"--work={self.hdl_library}"]
+                + self.build_args
+                + [self.hdl_toplevel]
+            ]
 
-        return cmd
+        return cmds
 
-    def test_command(self) -> List[Command]:
+    def _test_command(self) -> List[Command]:
 
-        cmd = [
+        cmds = [
             ["ghdl", "-r"]
-            + [self.sim_toplevel]
+            + [f"--work={self.hdl_toplevel_library}"]
+            + self.test_args
+            + [self.sim_hdl_toplevel]
             + ["--vpi=" + cocotb.config.lib_name_path("vpi", "ghdl")]
-            + self.sim_args
-            + self.get_parameter_options(self.parameters)
+            + self.plusargs
+            + self._get_parameter_options(self.parameters)
         ]
 
-        return cmd
+        return cmds
 
 
 class Riviera(Simulator):
+    supported_gpi_interfaces = {"verilog": ["vpi"], "vhdl": ["vhpi"]}
+
     @staticmethod
-    def simulator_in_path() -> None:
+    def _simulator_in_path() -> None:
         if shutil.which("vsimsa") is None:
             raise SystemExit("ERROR: vsimsa executable not found!")
 
-    def check_toplevel_lang(self, toplevel_lang: Optional[str]) -> str:
-        if toplevel_lang is None:
-            if self.vhdl_sources and not self.verilog_sources:
-                return "vhdl"
-            elif self.verilog_sources and not self.vhdl_sources:
-                return "verilog"
-            else:
-                raise ValueError(
-                    "Must specify a toplevel_lang in a mixed-language design"
-                )
-        elif toplevel_lang in ("verilog", "vhdl"):
-            return toplevel_lang
-        else:
-            raise ValueError(
-                f"Riviera does not support {toplevel_lang!r} as a toplevel_lang"
-            )
-
     @staticmethod
-    def get_include_options(includes: Sequence[str]) -> List[str]:
-        return ["+incdir+" + as_tcl_value(dir) for dir in includes]
+    def _get_include_options(includes: Sequence[PathLike]) -> Command:
+        return [f"+incdir+{as_tcl_value(str(include))}" for include in includes]
 
     @staticmethod
-    def get_define_options(defines: Sequence[str]) -> List[str]:
-        return ["+define+" + as_tcl_value(define) for define in defines]
+    def _get_define_options(defines: Mapping[str, object]) -> Command:
+        return [
+            f"+define+{as_tcl_value(name)}={as_tcl_value(str(value))}"
+            for name, value in defines.items()
+        ]
 
     @staticmethod
-    def get_parameter_options(parameters: Mapping[str, object]) -> List[str]:
-        return ["-g" + name + "=" + str(value) for name, value in parameters.items()]
+    def _get_parameter_options(parameters: Mapping[str, object]) -> Command:
+        return [f"-g{name}={value}" for name, value in parameters.items()]
 
-    def build_command(self) -> List[Command]:
+    def _build_command(self) -> List[Command]:
 
         do_script = "\nonerror {\n quit -code 1 \n} \n"
 
-        out_file = os.path.join(
-            self.build_dir, self.library_name, self.library_name + ".lib"
-        )
+        out_file = self.build_dir / self.hdl_library / f"{self.hdl_library}.lib"
 
         if outdated(out_file, self.verilog_sources + self.vhdl_sources) or self.always:
 
             do_script += "alib {RTL_LIBRARY} \n".format(
-                RTL_LIBRARY=as_tcl_value(self.library_name)
+                RTL_LIBRARY=as_tcl_value(self.hdl_library)
             )
 
             if self.vhdl_sources:
                 do_script += (
                     "acom -work {RTL_LIBRARY} {EXTRA_ARGS} {VHDL_SOURCES}\n".format(
-                        RTL_LIBRARY=as_tcl_value(self.library_name),
+                        RTL_LIBRARY=as_tcl_value(self.hdl_library),
                         VHDL_SOURCES=" ".join(
-                            as_tcl_value(v) for v in self.vhdl_sources
+                            as_tcl_value(str(v)) for v in self.vhdl_sources
                         ),
-                        EXTRA_ARGS=" ".join(as_tcl_value(v) for v in self.compile_args),
+                        EXTRA_ARGS=" ".join(as_tcl_value(v) for v in self.build_args),
                     )
                 )
 
             if self.verilog_sources:
                 do_script += "alog -work {RTL_LIBRARY} +define+COCOTB_SIM -sv {DEFINES} {INCDIR} {EXTRA_ARGS} {VERILOG_SOURCES} \n".format(
-                    RTL_LIBRARY=as_tcl_value(self.library_name),
+                    RTL_LIBRARY=as_tcl_value(self.hdl_library),
                     VERILOG_SOURCES=" ".join(
-                        as_tcl_value(v) for v in self.verilog_sources
+                        as_tcl_value(str(v)) for v in self.verilog_sources
                     ),
-                    DEFINES=" ".join(self.get_define_options(self.defines)),
-                    INCDIR=" ".join(self.get_include_options(self.includes)),
-                    EXTRA_ARGS=" ".join(as_tcl_value(v) for v in self.compile_args),
+                    DEFINES=" ".join(self._get_define_options(self.defines)),
+                    INCDIR=" ".join(self._get_include_options(self.includes)),
+                    EXTRA_ARGS=" ".join(as_tcl_value(v) for v in self.build_args),
                 )
         else:
-            print("WARNING: Skipping compilation:" + out_file)
+            print("WARNING: Skipping compilation of", out_file)
 
         do_file = tempfile.NamedTemporaryFile(delete=False)
         do_file.write(do_script.encode())
         do_file.close()
 
         return [["vsimsa"] + ["-do"] + ["do"] + [do_file.name]]
 
-    def test_command(self) -> List[Command]:
+    def _test_command(self) -> List[Command]:
 
         do_script = "\nonerror {\n quit -code 1 \n} \n"
 
-        if self.toplevel_lang == "vhdl":
-            do_script += "asim +access +w -interceptcoutput -O2 -loadvhpi {EXT_NAME} {EXTRA_ARGS} {TOPLEVEL} \n".format(
-                TOPLEVEL=as_tcl_value(self.sim_toplevel),
+        if self.hdl_toplevel_lang == "vhdl":
+            do_script += "asim +access +w -interceptcoutput -O2 -loadvhpi {EXT_NAME} {EXTRA_ARGS} {TOPLEVEL} {PLUSARGS}\n".format(
+                TOPLEVEL=as_tcl_value(
+                    f"{self.hdl_toplevel_library}.{self.sim_hdl_toplevel}"
+                ),
                 EXT_NAME=as_tcl_value(cocotb.config.lib_name_path("vhpi", "riviera")),
                 EXTRA_ARGS=" ".join(
                     as_tcl_value(v)
                     for v in (
-                        self.sim_args + self.get_parameter_options(self.parameters)
+                        self.test_args + self._get_parameter_options(self.parameters)
                     )
                 ),
+                PLUSARGS=" ".join(as_tcl_value(v) for v in self.plusargs),
             )
 
             self.env["GPI_EXTRA"] = (
                 cocotb.config.lib_name_path("vpi", "riviera") + ":cocotbvpi_entry_point"
             )
         else:
-            do_script += "asim +access +w -interceptcoutput -O2 -pli {EXT_NAME} {EXTRA_ARGS} {TOPLEVEL} {PLUS_ARGS} \n".format(
-                TOPLEVEL=as_tcl_value(self.sim_toplevel),
+            do_script += "asim +access +w -interceptcoutput -O2 -pli {EXT_NAME} {EXTRA_ARGS} {TOPLEVEL} {PLUSARGS} \n".format(
+                TOPLEVEL=as_tcl_value(
+                    f"{self.hdl_toplevel_library}.{self.sim_hdl_toplevel}"
+                ),
                 EXT_NAME=as_tcl_value(cocotb.config.lib_name_path("vpi", "riviera")),
                 EXTRA_ARGS=" ".join(
                     as_tcl_value(v)
                     for v in (
-                        self.sim_args + self.get_parameter_options(self.parameters)
+                        self.test_args + self._get_parameter_options(self.parameters)
                     )
                 ),
-                PLUS_ARGS=" ".join(as_tcl_value(v) for v in self.plus_args),
+                PLUSARGS=" ".join(as_tcl_value(v) for v in self.plusargs),
             )
 
             self.env["GPI_EXTRA"] = (
                 cocotb.config.lib_name_path("vhpi", "riviera")
                 + ":cocotbvhpi_entry_point"
             )
 
@@ -716,233 +797,237 @@
         do_file.write(do_script.encode())
         do_file.close()
 
         return [["vsimsa"] + ["-do"] + ["do"] + [do_file.name]]
 
 
 class Verilator(Simulator):
-    def simulator_in_path(self) -> None:
+    supported_gpi_interfaces = {"verilog": ["vpi"]}
+
+    def _simulator_in_path(self) -> None:
         executable = shutil.which("verilator")
         if executable is None:
             raise SystemExit("ERROR: verilator executable not found!")
-        self.executable = executable
+        self.executable: str = executable
 
     @staticmethod
-    def check_toplevel_lang(toplevel_lang: Optional[str]) -> str:
-        if toplevel_lang is None or toplevel_lang == "verilog":
-            return "verilog"
-        else:
-            raise ValueError(
-                f"Verilator does not support {toplevel_lang!r} as a toplevel_lang"
-            )
-
-    @staticmethod
-    def get_include_options(includes: Sequence[str]) -> List[str]:
-        return ["-I" + dir for dir in includes]
+    def _get_include_options(includes: Sequence[PathLike]) -> Command:
+        return [f"-I{include}" for include in includes]
 
     @staticmethod
-    def get_define_options(defines: Sequence[str]) -> List[str]:
-        return ["-D" + define for define in defines]
+    def _get_define_options(defines: Mapping[str, object]) -> Command:
+        return [f"-D{name}={value}" for name, value in defines.items()]
 
     @staticmethod
-    def get_parameter_options(parameters: Mapping[str, object]) -> List[str]:
-        return ["-G" + name + "=" + str(value) for name, value in parameters.items()]
+    def _get_parameter_options(parameters: Mapping[str, object]) -> Command:
+        return [f"-G{name}={value}" for name, value in parameters.items()]
 
-    def build_command(self) -> List[Command]:
+    def _build_command(self) -> List[Command]:
 
         if self.vhdl_sources:
-            raise ValueError("This simulator does not support VHDL")
+            raise ValueError(
+                f"{type(self).__qualname__}: Simulator does not support VHDL"
+            )
 
         if self.hdl_toplevel is None:
             raise ValueError(
-                "This simulator requires hdl_toplevel parameter to be specified"
+                f"{type(self).__qualname__}: Simulator requires the hdl_toplevel parameter to be specified"
             )
 
-        cmd = []
+        # TODO: set "--debug" if self.verbose
+        # TODO: support "--always"
 
-        verilator_cpp = os.path.join(
-            os.path.dirname(cocotb.__file__),
-            "share",
-            "lib",
-            "verilator",
-            "verilator.cpp",
+        verilator_cpp = str(
+            Path(cocotb.__file__).parent
+            / "share"
+            / "lib"
+            / "verilator"
+            / "verilator.cpp"
         )
 
-        cmd.append(
+        cmds = []
+        cmds.append(
             [
                 "perl",
                 self.executable,
                 "-cc",
                 "--exe",
                 "-Mdir",
-                self.build_dir,
+                str(self.build_dir),
                 "-DCOCOTB_SIM=1",
                 "--top-module",
                 self.hdl_toplevel,
                 "--vpi",
                 "--public-flat-rw",
                 "--prefix",
                 "Vtop",
                 "-o",
                 self.hdl_toplevel,
                 "-LDFLAGS",
                 "-Wl,-rpath,{LIB_DIR} -L{LIB_DIR} -lcocotbvpi_verilator".format(
                     LIB_DIR=cocotb.config.libs_dir
                 ),
             ]
-            + self.compile_args
-            + self.get_define_options(self.defines)
-            + self.get_include_options(self.includes)
-            + self.get_parameter_options(self.parameters)
+            + self.build_args
+            + self._get_define_options(self.defines)
+            + self._get_include_options(self.includes)
+            + self._get_parameter_options(self.parameters)
             + [verilator_cpp]
-            + self.verilog_sources
+            + [str(source_file) for source_file in self.verilog_sources]
         )
 
-        cmd.append(["make", "-C", self.build_dir, "-f", "Vtop.mk"])
+        cmds.append(["make", "-C", str(self.build_dir), "-f", "Vtop.mk"])
 
-        return cmd
+        return cmds
 
-    def test_command(self) -> List[Command]:
-        out_file = os.path.join(self.build_dir, self.sim_toplevel)
-        return [[out_file] + self.plus_args]
+    def _test_command(self) -> List[Command]:
+        out_file = self.build_dir / self.sim_hdl_toplevel
+        return [[str(out_file)] + self.plusargs]
 
 
 class Xcelium(Simulator):
+    supported_gpi_interfaces = {"verilog": ["vpi"], "vhdl": ["vhpi"]}
+
     @staticmethod
-    def simulator_in_path() -> None:
+    def _simulator_in_path() -> None:
         if shutil.which("xrun") is None:
             raise SystemExit("ERROR: xrun executable not found!")
 
-    def check_toplevel_lang(self, toplevel_lang: Optional[str]) -> str:
-        if toplevel_lang is None:
-            if self.vhdl_sources and not self.verilog_sources:
-                return "vhdl"
-            elif self.verilog_sources and not self.vhdl_sources:
-                return "verilog"
-            else:
-                raise ValueError("Must specify a toplevel_lang in a mixed design")
-        elif toplevel_lang in ("verilog", "vhdl"):
-            return toplevel_lang
-        else:
-            raise ValueError(
-                f"Xcelium does not support {toplevel_lang!r} as a toplevel_lang"
-            )
-
     @staticmethod
-    def get_include_options(includes: Sequence[str]) -> List[str]:
+    def _get_include_options(includes: Sequence[PathLike]) -> Command:
         return [f"-incdir {include}" for include in includes]
 
     @staticmethod
-    def get_define_options(defines: Sequence[str]) -> List[str]:
-        return [f"-define {define}" for define in defines]
+    def _get_define_options(defines: Mapping[str, object]) -> Command:
+        return [f"-define {name}={value}" for name, value in defines.items()]
 
     @staticmethod
-    def get_parameter_options(parameters: Mapping[str, object]) -> List[str]:
+    def _get_parameter_options(parameters: Mapping[str, object]) -> Command:
         return [f'-gpg "{name} => {value}"' for name, value in parameters.items()]
 
-    def build_command(self) -> List[Command]:
-
+    def _build_command(self) -> List[Command]:
         self.env["CDS_AUTO_64BIT"] = "all"
-        cmd = [
+
+        verbosity_opts = []
+        if self.verbose:
+            verbosity_opts += ["-messages"]
+            verbosity_opts += ["-status"]
+            verbosity_opts += ["-gverbose"]  # print assigned generics/parameters
+            verbosity_opts += ["-pliverbose"]
+            verbosity_opts += ["-plidebug"]  # Enhance the profile output with PLI info
+            verbosity_opts += [
+                "-plierr_verbose"
+            ]  # Expand handle info in PLI/VPI/VHPI messages
+
+        else:
+            verbosity_opts += ["-quiet"]
+            verbosity_opts += ["-plinowarn"]
+
+        cmds = [
             ["xrun"]
-            + ["-logfile xrun_build.log"]
+            + ["-logfile"]
+            + ["xrun_build.log"]
             + ["-elaborate"]
-            + [f"-xmlibdirname {self.build_dir}/xrun_snapshot"]
+            + ["-xmlibdirname"]
+            + [f"{self.build_dir}/xrun_snapshot"]
             + ["-licqueue"]
-            # TODO: way to switch to these verbose messages?:
-            + ["-messages"]
-            + ["-gverbose"]  # print assigned generics/parameters
-            + ["-plinowarn"]
-            # + ["-pliverbose"]
-            # + ["-plidebug"]  # Enhance the profile output with PLI info
-            # + ["-plierr_verbose"]  # Expand handle info in PLI/VPI/VHPI messages
+            + (["-clean"] if self.always else [])
+            + verbosity_opts
             # + ["-vpicompat 1800v2005"]  # <1364v1995|1364v2001|1364v2005|1800v2005> Specify the IEEE VPI
             + ["-access +rwc"]
+            + ["-loadvpi"]
+            # always start with VPI on Xcelium
             + [
-                "-loadvpi "
-                + cocotb.config.lib_name_path("vpi", "xcelium")
+                cocotb.config.lib_name_path("vpi", "xcelium")
                 + ":vlog_startup_routines_bootstrap"
             ]
-            + [f"-work {self.library_name}"]
-            + self.compile_args
+            + [f"-work {self.hdl_library}"]
+            + self.build_args
             + ["-define COCOTB_SIM"]
-            + self.get_define_options(self.defines)
-            + self.get_include_options(self.includes)
-            + self.get_parameter_options(self.parameters)
+            + self._get_include_options(self.includes)
+            + self._get_define_options(self.defines)
+            + self._get_parameter_options(self.parameters)
             + [f"-top {self.hdl_toplevel}"]
-            + self.vhdl_sources
-            + self.verilog_sources
+            + [
+                str(source_file)
+                for source_file in self.vhdl_sources + self.verilog_sources
+            ]
         ]
 
-        return cmd
+        return cmds
 
-    def test_command(self) -> List[Command]:
+    def _test_command(self) -> List[Command]:
         self.env["CDS_AUTO_64BIT"] = "all"
 
+        verbosity_opts = []
+        if self.verbose:
+            verbosity_opts += ["-messages"]
+            verbosity_opts += ["-status"]
+            verbosity_opts += ["-gverbose"]  # print assigned generics/parameters
+            verbosity_opts += ["-pliverbose"]
+            verbosity_opts += ["-plidebug"]  # Enhance the profile output with PLI info
+            verbosity_opts += [
+                "-plierr_verbose"
+            ]  # Expand handle info in PLI/VPI/VHPI messages
+
+        else:
+            verbosity_opts += ["-quiet"]
+            verbosity_opts += ["-plinowarn"]
+
         tmpdir = f"implicit_tmpdir_{self.current_test_name}"
-        cmd = [["mkdir", "-p", tmpdir]]
 
-        cmd += [
+        if self.hdl_toplevel_lang == "vhdl":
+            xrun_top = ":"
+        else:
+            xrun_top = self.sim_hdl_toplevel
+
+        cmds = [["mkdir", "-p", tmpdir]]
+        cmds += [
             ["xrun"]
-            + [f"-logfile xrun_{self.current_test_name}.log"]
-            + [
-                f"-xmlibdirname {self.build_dir}/xrun_snapshot -cds_implicit_tmpdir {tmpdir}"
-            ]
+            + ["-logfile"]
+            + [f"xrun_{self.current_test_name}.log"]
+            + ["-xmlibdirname"]
+            + [f"{self.build_dir}/xrun_snapshot"]
+            + ["-cds_implicit_tmpdir"]
+            + [tmpdir]
             + ["-licqueue"]
-            # TODO: way to switch to these verbose messages?:
-            + ["-messages"]
-            + ["-plinowarn"]
-            # + ["-pliverbose"]
-            # + ["-plidebug"]  # Enhance the profile output with PLI info
-            # + ["-plierr_verbose"]  # Expand handle info in PLI/VPI/VHPI messages
-            # + ["-vpicompat 1800v2005"]  # <1364v1995|1364v2001|1364v2005|1800v2005> Specify the IEEE VPI
+            + verbosity_opts
             + ["-R"]
-            + self.sim_args
-            + self.plus_args
+            + self.test_args
+            + self.plusargs
             + ["-gui" if self.gui else ""]
+            + ["-input"]
             + [
-                '-input "@probe -create {self.sim_toplevel} -all -depth all"'
+                f'-input "@database -open cocotb_waves -default" '
+                f'-input "@probe -database cocotb_waves -create {xrun_top} -all -depth all" '
+                f'-input "@run" '
+                f'-input "@exit" '
                 if self.waves
-                else ""
+                else "@run; exit;"
             ]
         ]
         self.env["GPI_EXTRA"] = (
             cocotb.config.lib_name_path("vhpi", "xcelium") + ":cocotbvhpi_entry_point"
         )
 
-        return cmd
+        return cmds
 
 
-def get_runner(simulator_name: str) -> Type[Simulator]:
+def get_runner(simulator_name: str) -> Simulator:
+    """Return the *simulator_name* instance."""
 
-    sim_name = simulator_name.lower()
     supported_sims: Dict[str, Type[Simulator]] = {
         "icarus": Icarus,
         "questa": Questa,
         "ghdl": Ghdl,
         "riviera": Riviera,
         "verilator": Verilator,
         "xcelium": Xcelium,
         # TODO: "vcs": Vcs,
+        # TODO: "activehdl": ActiveHdl,
     }
     try:
-        return supported_sims[sim_name]
+        return supported_sims[simulator_name]()
     except KeyError:
-        raise NotImplementedError(
-            "Set SIM variable. Supported: " + ", ".join(supported_sims)
+        raise ValueError(
+            f"Simulator {simulator_name!r} is not in supported list: {', '.join(supported_sims)}"
         ) from None
-
-
-def clean(recursive: bool = False) -> None:
-    dir = os.getcwd()
-
-    def rm_clean() -> None:
-        build_dir = os.path.join(dir, "sim_build")
-        if os.path.isdir(build_dir):
-            print("INFO: Removing:", build_dir)
-            shutil.rmtree(build_dir, ignore_errors=True)
-
-    rm_clean()
-
-    if recursive:
-        for dir, _, _ in os.walk(dir):
-            rm_clean()
```

### Comparing `cocotb-1.7.2/cocotb/scheduler.py` & `cocotb-1.8.0rc1/cocotb/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 from contextlib import contextmanager
 from typing import Any, Callable, Union
 
 import cocotb
 import cocotb.decorators
 from cocotb import _py_compat, outcomes
 from cocotb._deprecation import deprecated
-from cocotb.decorators import Task
 from cocotb.log import SimLog
 from cocotb.result import TestComplete
+from cocotb.task import Task
 from cocotb.triggers import (
     Event,
     GPITrigger,
     Join,
     NextTimeStep,
     NullTrigger,
     ReadOnly,
@@ -72,15 +72,15 @@
     _profile = cProfile.Profile()
 
 # Sadly the Python standard logging module is very slow so it's better not to
 # make any calls by testing a boolean flag first
 _debug = "COCOTB_SCHEDULER_DEBUG" in os.environ
 
 
-class InternalError(RuntimeError):
+class InternalError(BaseException):
     """An error internal to scheduler. If you see this, report a bug!"""
 
     pass
 
 
 class profiling_context:
     """Context manager that profiles its contents"""
@@ -261,14 +261,15 @@
         # Only the last scheduled write to a particular handle in a timestep is performed.
         self._write_calls = OrderedDict()
 
         self._pending_coros = []
         self._pending_triggers = []
         self._pending_threads = []
         self._pending_events = []  # Events we need to call set on once we've unwound
+        self._scheduling = []
 
         self._terminate = False
         self._test = None
         self._main_thread = threading.current_thread()
 
         self._current_task = None
 
@@ -433,15 +434,15 @@
 
                 # this only exists to enable the warning above
                 is_first = False
 
                 # Scheduled coroutines may append to our waiting list so the first
                 # thing to do is pop all entries waiting on this trigger.
                 try:
-                    scheduling = self._trigger2coros.pop(trigger)
+                    self._scheduling = self._trigger2coros.pop(trigger)
                 except KeyError:
                     # GPI triggers should only be ever pending if there is an
                     # associated coroutine waiting on that trigger, otherwise it would
                     # have been unprimed already
                     if isinstance(trigger, GPITrigger):
                         self.log.critical(
                             "No coroutines waiting on trigger that fired: %s"
@@ -459,27 +460,27 @@
                         )
 
                     del trigger
                     continue
 
                 if _debug:
                     debugstr = "\n\t".join(
-                        [coro._coro.__qualname__ for coro in scheduling]
+                        [coro._coro.__qualname__ for coro in self._scheduling]
                     )
-                    if len(scheduling) > 0:
+                    if len(self._scheduling) > 0:
                         debugstr = "\n\t" + debugstr
                     self.log.debug(
                         "%d pending coroutines for event %s%s"
-                        % (len(scheduling), str(trigger), debugstr)
+                        % (len(self._scheduling), str(trigger), debugstr)
                     )
 
                 # This trigger isn't needed any more
                 trigger.unprime()
 
-                for coro in scheduling:
+                for coro in self._scheduling:
                     if coro._outcome is not None:
                         # coroutine was killed by another coroutine waiting on the same trigger
                         continue
                     if _debug:
                         self.log.debug(
                             "Scheduling coroutine %s" % (coro._coro.__qualname__)
                         )
@@ -490,14 +491,16 @@
                         )
 
                     # remove our reference to the objects at the end of each loop,
                     # to try and avoid them being destroyed at a weird time (as
                     # happened in gh-957)
                     del coro
 
+                self._scheduling = []
+
                 # Handle any newly queued coroutines that need to be scheduled
                 while self._pending_coros:
                     task = self._pending_coros.pop(0)
                     if _debug:
                         self.log.debug(
                             "Scheduling queued coroutine %s" % (task._coro.__qualname__)
                         )
@@ -518,15 +521,14 @@
                         )
                     self._pending_events.pop(0).set()
 
                 # remove our reference to the objects at the end of each loop,
                 # to try and avoid them being destroyed at a weird time (as
                 # happened in gh-957)
                 del trigger
-                del scheduling
 
             # no more pending triggers
             self._check_termination()
             if _debug:
                 self.log.debug(
                     "All coroutines scheduled, handing control back" " to simulator"
                 )
@@ -575,15 +577,15 @@
                 # throws an error if the background coroutine errored
                 # and no one was monitoring it
                 coro._outcome.get()
             except (TestComplete, AssertionError) as e:
                 coro.log.info("Test stopped by this forked coroutine")
                 e = remove_traceback_frames(e, ["_unschedule", "get"])
                 self._abort_test(e)
-            except Exception as e:
+            except BaseException as e:
                 coro.log.error("Exception raised by this forked coroutine")
                 e = remove_traceback_frames(e, ["_unschedule", "get"])
                 warnings.warn(
                     '"Unwatched" tasks that throw exceptions will not cause the test to fail. '
                     "See issue #2664 for more details.",
                     FutureWarning,
                 )
@@ -617,15 +619,14 @@
             # this coroutine.
             trigger_coros.insert(0, coro)
         else:
             # Everything else joins the back of the queue
             trigger_coros.append(coro)
 
         if not trigger.primed:
-
             if trigger_coros != [coro]:
                 # should never happen
                 raise InternalError(
                     "More than one coroutine waiting on an unprimed trigger"
                 )
 
             try:
@@ -692,15 +693,15 @@
             # calling thread_suspend.
             # We need to do this here in the scheduler thread so that no more
             # coroutines run until the background thread goes back to sleep.
             t.thread_resume()
             event.set()
 
         event = threading.Event()
-        self._pending_coros.append(cocotb.decorators.Task(wrapper()))
+        self._pending_coros.append(Task(wrapper()))
         # The scheduler thread blocks in `thread_wait`, and is woken when we
         # call `thread_suspend` - so we need to make sure the coroutine is
         # queued before that.
         t.thread_suspend()
         # This blocks the calling `@external` thread until the coroutine finishes
         event.wait()
         return event.outcome.get()
@@ -845,50 +846,50 @@
 
     # This collection of functions parses a trigger out of the object
     # that was yielded by a coroutine, converting `list` -> `Waitable`,
     # `Waitable` -> `Task`, `Task` -> `Trigger`.
     # Doing them as separate functions allows us to avoid repeating unnecessary
     # `isinstance` checks.
 
-    def _trigger_from_started_coro(self, result: cocotb.decorators.Task) -> Trigger:
+    def _trigger_from_started_coro(self, result: Task) -> Trigger:
         if _debug:
             self.log.debug(
                 "Joining to already running coroutine: %s" % result._coro.__qualname__
             )
         return result.join()
 
-    def _trigger_from_unstarted_coro(self, result: cocotb.decorators.Task) -> Trigger:
+    def _trigger_from_unstarted_coro(self, result: Task) -> Trigger:
         self._queue(result)
         if _debug:
             self.log.debug(
                 "Scheduling nested coroutine: %s" % result._coro.__qualname__
             )
         return result.join()
 
     def _trigger_from_waitable(self, result: cocotb.triggers.Waitable) -> Trigger:
-        return self._trigger_from_unstarted_coro(cocotb.decorators.Task(result._wait()))
+        return self._trigger_from_unstarted_coro(Task(result._wait()))
 
     def _trigger_from_list(self, result: list) -> Trigger:
         return self._trigger_from_waitable(cocotb.triggers.First(*result))
 
     def _trigger_from_any(self, result) -> Trigger:
         """Convert a yielded object into a Trigger instance"""
         # note: the order of these can significantly impact performance
 
         if isinstance(result, Trigger):
             return result
 
-        if isinstance(result, cocotb.decorators.Task):
+        if isinstance(result, Task):
             if not result.has_started():
                 return self._trigger_from_unstarted_coro(result)
             else:
                 return self._trigger_from_started_coro(result)
 
         if inspect.iscoroutine(result):
-            return self._trigger_from_unstarted_coro(cocotb.decorators.Task(result))
+            return self._trigger_from_unstarted_coro(Task(result))
 
         if isinstance(result, list):
             return self._trigger_from_list(result)
 
         if isinstance(result, cocotb.triggers.Waitable):
             return self._trigger_from_waitable(result)
 
@@ -975,15 +976,14 @@
                 self._resume_coro_upon(coroutine, result)
 
             # We do not return from here until pending threads have completed, but only
             # from the main thread, this seems like it could be problematic in cases
             # where a sim might change what this thread is.
 
             if self._main_thread is threading.current_thread():
-
                 for ext in self._pending_threads:
                     ext.thread_start()
                     if _debug:
                         self.log.debug(
                             "Blocking from {} on {}".format(
                                 threading.current_thread(), ext.thread
                             )
@@ -1058,26 +1058,43 @@
 
     def _cleanup(self):
         """Clear up all our state.
 
         Unprime all pending triggers and kill off any coroutines, stop all externals.
         """
         # copy since we modify this in kill
-        items = list(self._trigger2coros.items())
+        items = list((k, list(v)) for k, v in self._trigger2coros.items())
 
         # reversing seems to fix gh-928, although the order is still somewhat
         # arbitrary.
         for trigger, waiting in items[::-1]:
             for coro in waiting:
                 if _debug:
                     self.log.debug("Killing %s" % str(coro))
                 coro.kill()
+        assert not self._trigger2coros
+
+        # if there are coroutines being scheduled when the test ends, kill them (gh-1347)
+        for coro in self._scheduling:
+            if _debug:
+                self.log.debug("Killing %s" % str(coro))
+            coro.kill()
+        self._scheduling = []
+
+        # cancel outstanding triggers *before* queued coroutines (gh-3270)
+        while self._pending_triggers:
+            trigger = self._pending_triggers.pop(0)
+            if _debug:
+                self.log.debug("Unpriming %r", trigger)
+            trigger.unprime()
+        assert not self._pending_triggers
 
         # kill any queued coroutines
         for task in self._pending_coros:
             task.kill()
+        assert not self._pending_coros
 
         if self._main_thread is not threading.current_thread():
             raise Exception("Cleanup() called outside of the main thread")
 
         for ext in self._pending_threads:
             self.log.warning("Waiting for %s to exit", ext.thread)
```

### Comparing `cocotb-1.7.2/cocotb/share/def/aldec.def` & `cocotb-1.8.0rc1/cocotb/share/def/aldec.def`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/def/ghdl.def` & `cocotb-1.8.0rc1/cocotb/share/def/ghdl.def`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/def/icarus.def` & `cocotb-1.8.0rc1/cocotb/share/def/icarus.def`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/def/modelsim.def` & `cocotb-1.8.0rc1/cocotb/share/def/modelsim.def`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 mti_NextRegion
 mti_NextSignal
 mti_NextVar
 mti_Now
 mti_NowUpper
 mti_Quit
 mti_ReleaseSignal
+mti_RemoveLoadDoneCB
+mti_RemoveQuitCB
 mti_ScheduleWakeup
 mti_ScheduleWakeup64
 mti_Sensitize
 mti_SetSignalValue
 mti_SetVarValue
 mti_TickLeft
 mti_TickLength
```

### Comparing `cocotb-1.7.2/cocotb/share/include/cocotb_utils.h` & `cocotb-1.8.0rc1/cocotb/share/include/cocotb_utils.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/include/embed.h` & `cocotb-1.8.0rc1/cocotb/share/include/embed.h`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 extern "C" {
 #endif
 
 extern COCOTB_EMBED_EXPORT void embed_init_python(void);
 extern COCOTB_EMBED_EXPORT void embed_sim_cleanup(void);
 extern COCOTB_EMBED_EXPORT int embed_sim_init(int argc,
                                               char const* const* argv);
-extern COCOTB_EMBED_EXPORT void embed_sim_event(gpi_event_t level,
-                                                const char* msg);
+extern COCOTB_EMBED_EXPORT void embed_sim_event(const char* msg);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* COCOTB_EMBED_H_ */
```

### Comparing `cocotb-1.7.2/cocotb/share/include/exports.h` & `cocotb-1.8.0rc1/cocotb/share/include/exports.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/include/gpi.h` & `cocotb-1.8.0rc1/cocotb/share/include/gpi.h`

 * *Files 3% similar despite different names*

```diff
@@ -97,20 +97,14 @@
 typedef struct GpiIterator *gpi_iterator_hdl;
 #endif
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-typedef enum gpi_event_e {
-    SIM_INFO = 0,
-    SIM_TEST_FAIL = 1,
-    SIM_FAIL = 2,
-} gpi_event_t;
-
 // Functions for controlling/querying the simulation state
 
 /**
  * Returns 1 if there is a registered GPI implementation, 0 otherwise.
  *
  * Useful for checking if a simulator is running.
  */
@@ -238,25 +232,26 @@
 
 typedef enum gpi_edge {
     GPI_RISING = 1,
     GPI_FALLING = 2,
 } gpi_edge_e;
 
 // The callback registering functions
-GPI_EXPORT gpi_cb_hdl gpi_register_timed_callback(
-    int (*gpi_function)(const void *), void *gpi_cb_data, uint64_t time);
+GPI_EXPORT gpi_cb_hdl gpi_register_timed_callback(int (*gpi_function)(void *),
+                                                  void *gpi_cb_data,
+                                                  uint64_t time);
 GPI_EXPORT gpi_cb_hdl gpi_register_value_change_callback(
-    int (*gpi_function)(const void *), void *gpi_cb_data, gpi_sim_hdl gpi_hdl,
+    int (*gpi_function)(void *), void *gpi_cb_data, gpi_sim_hdl gpi_hdl,
     int edge);
-GPI_EXPORT gpi_cb_hdl gpi_register_readonly_callback(
-    int (*gpi_function)(const void *), void *gpi_cb_data);
-GPI_EXPORT gpi_cb_hdl gpi_register_nexttime_callback(
-    int (*gpi_function)(const void *), void *gpi_cb_data);
-GPI_EXPORT gpi_cb_hdl gpi_register_readwrite_callback(
-    int (*gpi_function)(const void *), void *gpi_cb_data);
+GPI_EXPORT gpi_cb_hdl
+gpi_register_readonly_callback(int (*gpi_function)(void *), void *gpi_cb_data);
+GPI_EXPORT gpi_cb_hdl
+gpi_register_nexttime_callback(int (*gpi_function)(void *), void *gpi_cb_data);
+GPI_EXPORT gpi_cb_hdl
+gpi_register_readwrite_callback(int (*gpi_function)(void *), void *gpi_cb_data);
 
 // Calling convention is that 0 = success and negative numbers a failure
 // For implementers of GPI the provided macro GPI_RET(x) is provided
 GPI_EXPORT void gpi_deregister_callback(gpi_cb_hdl gpi_hdl);
 
 // Because the internal structures may be different for different
 // implementations of GPI we provide a convenience function to extract the
```

### Comparing `cocotb-1.7.2/cocotb/share/include/gpi_logging.h` & `cocotb-1.8.0rc1/cocotb/share/include/gpi_logging.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/include/py_gpi_logging.h` & `cocotb-1.8.0rc1/cocotb/share/include/py_gpi_logging.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/include/vhpi_user_ext.h` & `cocotb-1.8.0rc1/cocotb/share/include/vhpi_user_ext.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/include/vpi_user_ext.h` & `cocotb-1.8.0rc1/cocotb/share/include/vpi_user_ext.h`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 #ifndef VPI_USER_EXT_H
 #define VPI_USER_EXT_H
 
 #ifdef  __cplusplus
 extern "C" {
 #endif
 
+/* used by Cadence Xcelium for packed unions */
+#define vpiUnionNet          525
+
 /* used by Cadence Xcelium for Verilog-AMS */
 #define vpiRealNet           526
 #define vpiInterconnectNet   533
 #define vpiInterconnectArray 534
 
 /* arguments for vpiStop or vpiFinish */
 #define vpiDiagNone               0  /* prints nothing */
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/embed/embed.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/embed/embed.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #else
 #define EMBED_IMPL_LIB_STR xstr(EMBED_IMPL_LIB)
 #endif
 
 static void (*_embed_init_python)();
 static void (*_embed_sim_cleanup)();
 static int (*_embed_sim_init)(int argc, char const *const *argv);
-static void (*_embed_sim_event)(gpi_event_t level, const char *msg);
+static void (*_embed_sim_event)(const char *msg);
 
 static bool init_failed = false;
 
 #ifdef _WIN32
 static ACTCTX act_ctx = {
     /* cbSize */ sizeof(ACTCTX),
     /* dwFlags */ ACTCTX_FLAG_HMODULE_VALID | ACTCTX_FLAG_RESOURCE_NAME_VALID,
@@ -157,12 +157,12 @@
         return -1;
         // LCOV_EXCL_STOP
     } else {
         return _embed_sim_init(argc, argv);
     }
 }
 
-extern "C" void embed_sim_event(gpi_event_t level, const char *msg) {
+extern "C" void embed_sim_event(const char *msg) {
     if (!init_failed) {
-        _embed_sim_event(level, msg);
+        _embed_sim_event(msg);
     }
 }
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/embed/gpi_embed.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/embed/gpi_embed.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 #include <cocotb_utils.h>  // DEFER
 #include <exports.h>       // COCOTB_EXPORT
 #include <gpi.h>           // gpi_event_t
 #include <gpi_logging.h>   // LOG_* macros
 #include <py_gpi_logging.h>  // py_gpi_logger_set_level, py_gpi_logger_initialize, py_gpi_logger_finalize
 
 #include <cassert>
+#include <string>
 
 #include "locale.h"
 
 #if defined(_WIN32)
 #include <windows.h>
 #define sleep(n) Sleep(1000 * n)
 #define getpid() GetCurrentProcessId()
@@ -53,60 +54,55 @@
 static PyThreadState *gtstate = NULL;
 
 static wchar_t progname[] = L"cocotb";
 static wchar_t *argv[] = {progname};
 
 #if defined(_WIN32)
 #if defined(__MINGW32__) || defined(__CYGWIN32__)
-const char *PYTHON_INTERPRETER_PATH = "/Scripts/python";
+constexpr char const *PYTHON_INTERPRETER_PATH = "/Scripts/python";
 #else
-const char *PYTHON_INTERPRETER_PATH = "\\Scripts\\python";
+constexpr char const *PYTHON_INTERPRETER_PATH = "\\Scripts\\python";
 #endif
 #else
-const char *PYTHON_INTERPRETER_PATH = "/bin/python";
+constexpr char const *PYTHON_INTERPRETER_PATH = "/bin/python";
 #endif
 
 static PyObject *pEventFn = NULL;
 
 static void set_program_name_in_venv(void) {
-    static char venv_path[PATH_MAX];
     static wchar_t venv_path_w[PATH_MAX];
 
     const char *venv_path_home = getenv("VIRTUAL_ENV");
     if (!venv_path_home) {
         LOG_INFO(
             "Did not detect Python virtual environment. "
             "Using system-wide Python interpreter");
         return;
     }
 
-    strncpy(venv_path, venv_path_home, sizeof(venv_path) - 1);
-    if (venv_path[sizeof(venv_path) - 1]) {
-        LOG_ERROR(
-            "Unable to set Python Program Name using virtual environment. "
-            "Path to virtual environment too long");
-        return;
-    }
+    std::string venv_path = venv_path_home;
+    venv_path.append(PYTHON_INTERPRETER_PATH);
 
-    strncat(venv_path, PYTHON_INTERPRETER_PATH,
-            sizeof(venv_path) - strlen(venv_path) - 1);
-    if (venv_path[sizeof(venv_path) - 1]) {
+    auto venv_path_w_temp = Py_DecodeLocale(venv_path.c_str(), NULL);
+    if (venv_path_w_temp == NULL) {
         LOG_ERROR(
             "Unable to set Python Program Name using virtual environment. "
-            "Path to interpreter too long");
+            "Decoding error in virtual environment path.");
+        LOG_INFO("Virtual environment path: %s", venv_path.c_str());
         return;
     }
+    DEFER(PyMem_RawFree(venv_path_w_temp));
 
-    wcsncpy(venv_path_w, Py_DecodeLocale(venv_path, NULL),
+    wcsncpy(venv_path_w, venv_path_w_temp,
             sizeof(venv_path_w) / sizeof(wchar_t));
-
     if (venv_path_w[(sizeof(venv_path_w) / sizeof(wchar_t)) - 1]) {
         LOG_ERROR(
             "Unable to set Python Program Name using virtual environment. "
             "Path to interpreter too long");
+        LOG_INFO("Virtual environment path: %s", venv_path.c_str());
         return;
     }
 
     LOG_INFO("Using Python virtual environment interpreter at %ls",
              venv_path_w);
     Py_SetProgramName(venv_path_w);
 }
@@ -123,14 +119,16 @@
  * Stores the thread state for cocotb in static variable gtstate
  */
 
 extern "C" COCOTB_EXPORT void _embed_init_python(void) {
     assert(!gtstate);  // this function should not be called twice
 
     to_python();
+    // must set program name to Python executable before initialization, so
+    // initialization can determine path from executable
     set_program_name_in_venv();
     Py_Initialize(); /* Initialize the interpreter */
     PySys_SetArgvEx(1, argv, 0);
 
     /* Swap out and return current thread state and release the GIL */
     gtstate = PyEval_SaveThread();
     to_simulator();
@@ -292,28 +290,27 @@
         // LCOV_EXCL_STOP
     }
     Py_DECREF(cocotb_retval);
 
     return 0;
 }
 
-extern "C" COCOTB_EXPORT void _embed_sim_event(gpi_event_t level,
-                                               const char *msg) {
+extern "C" COCOTB_EXPORT void _embed_sim_event(const char *msg) {
     /* Indicate to the upper layer that a sim event occurred */
 
     if (pEventFn) {
         PyGILState_STATE gstate;
         to_python();
         gstate = PyGILState_Ensure();
 
         if (msg == NULL) {
             msg = "No message provided";
         }
 
-        PyObject *pValue = PyObject_CallFunction(pEventFn, "ls", level, msg);
+        PyObject *pValue = PyObject_CallFunction(pEventFn, "s", msg);
         if (pValue == NULL) {
             PyErr_Print();
             LOG_ERROR("Passing event to upper layer failed");
         }
         Py_XDECREF(pValue);
         PyGILState_Release(gstate);
         to_simulator();
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/fli/FliCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliCbHdl.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,32 @@
  *
  * We keep the process but desensitize it
  *
  * NB: need a way to determine if should leave it sensitized...
  *
  */
 int FliProcessCbHdl::cleanup_callback() {
-    if (get_call_state() == GPI_PRIMED) {
-        mti_Desensitize(m_proc_hdl);
-        set_call_state(GPI_DELETE);
+    switch (get_call_state()) {
+        case GPI_PRIMED:
+        case GPI_CALL:
+            mti_Desensitize(m_proc_hdl);
+            set_call_state(GPI_DELETE);
+            break;
+        case GPI_DELETE:
+        case GPI_FREE:
+            break;
     }
     return 0;
 }
 
 FliTimedCbHdl::FliTimedCbHdl(GpiImplInterface* impl, uint64_t time)
-    : GpiCbHdl(impl), FliProcessCbHdl(impl), m_time(time) {
+    : GpiCbHdl(impl),
+      FliProcessCbHdl(impl),
+      GpiCommonCbHdl(impl),
+      m_time(time) {
     m_proc_hdl = mti_CreateProcessWithPriority(NULL, handle_fli_callback,
                                                (void*)this, MTI_PROC_IMMEDIATE);
 }
 
 int FliTimedCbHdl::arm_callback() {
 #if defined(__LP64__) || defined(_WIN64)
     mti_ScheduleWakeup64(m_proc_hdl, static_cast<mtiTime64T>(m_time));
@@ -121,14 +130,15 @@
     }
     return 0;
 }
 
 FliSignalCbHdl::FliSignalCbHdl(GpiImplInterface* impl, FliSignalObjHdl* sig_hdl,
                                int edge)
     : GpiCbHdl(impl),
+      GpiCommonCbHdl(impl),
       FliProcessCbHdl(impl),
       GpiValueCbHdl(impl, sig_hdl, edge) {
     m_sig_hdl = m_signal->get_handle<mtiSignalIdT>();
 }
 
 int FliStartupCbHdl::arm_callback() {
     mti_AddLoadDoneCB(handle_fli_callback, (void*)this);
@@ -192,19 +202,31 @@
     const char** argv = argv_cstr.data();
 
     gpi_embed_init(argc, argv);
 
     return 0;
 }
 
+int FliStartupCbHdl::cleanup_callback() {
+    mti_RemoveLoadDoneCB(handle_fli_callback, (void*)this);
+    set_call_state(GPI_DELETE);
+    return 0;
+}
+
 int FliShutdownCbHdl::arm_callback() {
     mti_AddQuitCB(handle_fli_callback, (void*)this);
     set_call_state(GPI_PRIMED);
 
     return 0;
 }
 
 int FliShutdownCbHdl::run_callback() {
     gpi_embed_end();
 
     return 0;
 }
+
+int FliShutdownCbHdl::cleanup_callback() {
+    mti_RemoveQuitCB(handle_fli_callback, (void*)this);
+    set_call_state(GPI_DELETE);
+    return 0;
+}
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/fli/FliImpl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -109,16 +109,17 @@
             type == accVariable || type == accSignal);
 }
 
 bool FliImpl::isTypeSignal(int type, int full_type) {
     return (type == accSignal || full_type == accAliasSignal);
 }
 
-GpiObjHdl *FliImpl::create_gpi_obj_from_handle(void *hdl, std::string &name,
-                                               std::string &fq_name,
+GpiObjHdl *FliImpl::create_gpi_obj_from_handle(void *hdl,
+                                               const std::string &name,
+                                               const std::string &fq_name,
                                                int accType, int accFullType) {
     GpiObjHdl *new_obj = NULL;
 
     LOG_DEBUG(
         "Attempting to create GPI object from handle (Type=%d, FullType=%d).",
         accType, accFullType);
     if (!VS_TYPE_IS_VHDL(accFullType)) {
@@ -266,15 +267,16 @@
 }
 
 /**
  * @name    Native Check Create
  * @brief   Determine whether a simulation object is native to FLI and create
  *          a handle if it is
  */
-GpiObjHdl *FliImpl::native_check_create(std::string &name, GpiObjHdl *parent) {
+GpiObjHdl *FliImpl::native_check_create(const std::string &name,
+                                        GpiObjHdl *parent) {
     bool search_rgn = false;
     bool search_sig = false;
     bool search_var = false;
 
     std::string fq_name = parent->get_fullname();
     gpi_objtype_t obj_type = parent->get_type();
 
@@ -558,43 +560,52 @@
 
         LOG_ERROR("FLI: Toplevel instances: %s != %s...", name,
                   mti_GetRegionName(root));
     }
     return NULL;
 }
 
-GpiCbHdl *FliImpl::register_timed_callback(uint64_t time) {
-    // get time from cache instead of allocating
+GpiCbHdl *FliImpl::register_timed_callback(uint64_t time,
+                                           int (*function)(void *),
+                                           void *cb_data) {
+    // get timer from cache instead of allocating
     FliTimedCbHdl *hdl = cache.get_timer(time);
 
     if (hdl->arm_callback()) {
         delete (hdl);
-        hdl = NULL;
+        return NULL;
     }
+    hdl->set_user_data(function, cb_data);
     return hdl;
 }
 
-GpiCbHdl *FliImpl::register_readonly_callback() {
+GpiCbHdl *FliImpl::register_readonly_callback(int (*function)(void *),
+                                              void *cb_data) {
     if (m_readonly_cbhdl.arm_callback()) {
         return NULL;
     }
+    m_readonly_cbhdl.set_user_data(function, cb_data);
     return &m_readonly_cbhdl;
 }
 
-GpiCbHdl *FliImpl::register_readwrite_callback() {
+GpiCbHdl *FliImpl::register_readwrite_callback(int (*function)(void *),
+                                               void *cb_data) {
     if (m_readwrite_cbhdl.arm_callback()) {
         return NULL;
     }
+    m_readwrite_cbhdl.set_user_data(function, cb_data);
     return &m_readwrite_cbhdl;
 }
 
-GpiCbHdl *FliImpl::register_nexttime_callback() {
+GpiCbHdl *FliImpl::register_nexttime_callback(int (*function)(void *),
+                                              void *cb_data) {
     if (m_nexttime_cbhdl.arm_callback()) {
         return NULL;
     }
+    m_nexttime_cbhdl.set_user_data(function, cb_data);
     return &m_nexttime_cbhdl;
 }
 
 int FliImpl::deregister_callback(GpiCbHdl *gpi_hdl) {
     return gpi_hdl->cleanup_callback();
 }
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/fli/FliImpl.h` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.h`

 * *Files 3% similar despite different names*

```diff
@@ -75,18 +75,21 @@
     }
 
   private:
     mtiSignalIdT m_sig_hdl;
 };
 
 // All other callbacks are related to the simulation phasing
-class FliSimPhaseCbHdl : public FliProcessCbHdl {
+class FliSimPhaseCbHdl : public FliProcessCbHdl, public GpiCommonCbHdl {
   public:
     FliSimPhaseCbHdl(GpiImplInterface *impl, mtiProcessPriorityT priority)
-        : GpiCbHdl(impl), FliProcessCbHdl(impl), m_priority(priority) {}
+        : GpiCbHdl(impl),
+          FliProcessCbHdl(impl),
+          GpiCommonCbHdl(impl),
+          m_priority(priority) {}
 
     int arm_callback() override;
 
   protected:
     mtiProcessPriorityT m_priority;
 };
 
@@ -112,26 +115,28 @@
 class FliStartupCbHdl : public FliProcessCbHdl {
   public:
     FliStartupCbHdl(GpiImplInterface *impl)
         : GpiCbHdl(impl), FliProcessCbHdl(impl) {}
 
     int arm_callback() override;
     int run_callback() override;
+    int cleanup_callback() override;
 };
 
 class FliShutdownCbHdl : public FliProcessCbHdl {
   public:
     FliShutdownCbHdl(GpiImplInterface *impl)
         : GpiCbHdl(impl), FliProcessCbHdl(impl) {}
 
     int arm_callback() override;
     int run_callback() override;
+    int cleanup_callback() override;
 };
 
-class FliTimedCbHdl : public FliProcessCbHdl {
+class FliTimedCbHdl : public FliProcessCbHdl, public GpiCommonCbHdl {
   public:
     FliTimedCbHdl(GpiImplInterface *impl, uint64_t time);
 
     int arm_callback() override;
     void reset_time(uint64_t new_time) { m_time = new_time; }
     int cleanup_callback() override;
 
@@ -158,30 +163,33 @@
 class FliObjHdl : public GpiObjHdl, public FliObj {
   public:
     FliObjHdl(GpiImplInterface *impl, void *hdl, gpi_objtype_t objtype,
               int acc_type, int acc_full_type, bool is_const = false)
         : GpiObjHdl(impl, hdl, objtype, is_const),
           FliObj(acc_type, acc_full_type) {}
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 };
 
 class FliSignalObjHdl : public GpiSignalObjHdl, public FliObj {
   public:
     FliSignalObjHdl(GpiImplInterface *impl, void *hdl, gpi_objtype_t objtype,
                     bool is_const, int acc_type, int acc_full_type, bool is_var)
         : GpiSignalObjHdl(impl, hdl, objtype, is_const),
           FliObj(acc_type, acc_full_type),
           m_is_var(is_var),
           m_rising_cb(impl, this, GPI_RISING),
           m_falling_cb(impl, this, GPI_FALLING),
           m_either_cb(impl, this, GPI_FALLING | GPI_RISING) {}
 
-    GpiCbHdl *value_change_cb(int edge) override;
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
+    GpiCbHdl *register_value_change_callback(int edge, int (*function)(void *),
+                                             void *cb_data) override;
 
     bool is_var() { return m_is_var; }
 
   protected:
     bool m_is_var;
     FliSignalCbHdl m_rising_cb;
     FliSignalCbHdl m_falling_cb;
@@ -213,15 +221,16 @@
     int set_signal_value_str(std::string &value,
                              gpi_set_action_t action) override;
     int set_signal_value_binstr(std::string &value,
                                 gpi_set_action_t action) override;
 
     void *get_sub_hdl(int index);
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 
     mtiTypeKindT get_fli_typekind() { return m_fli_type; }
     mtiTypeIdT get_fli_typeid() { return m_val_type; }
 
   protected:
     mtiTypeKindT m_fli_type;
     mtiTypeIdT m_val_type;
@@ -239,15 +248,16 @@
 
     const char *get_signal_value_str() override;
     long get_signal_value_long() override;
 
     using FliValueObjHdl::set_signal_value;
     int set_signal_value(int32_t value, gpi_set_action_t action) override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 
   private:
     char **m_value_enum = nullptr;  // Do Not Free
     mtiInt32T m_num_enum = 0;
 };
 
 class FliLogicObjHdl : public FliValueObjHdl {
@@ -265,15 +275,16 @@
     const char *get_signal_value_binstr() override;
 
     using FliValueObjHdl::set_signal_value;
     int set_signal_value(int32_t value, gpi_set_action_t action) override;
     int set_signal_value_binstr(std::string &value,
                                 gpi_set_action_t action) override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 
   private:
     char *m_mti_buff = nullptr;
     char **m_value_enum = nullptr;  // Do Not Free
     mtiInt32T m_num_enum = 0;
     std::map<char, mtiInt32T> m_enum_map;
 };
@@ -288,15 +299,16 @@
 
     const char *get_signal_value_binstr() override;
     long get_signal_value_long() override;
 
     using FliValueObjHdl::set_signal_value;
     int set_signal_value(int32_t value, gpi_set_action_t action) override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 };
 
 class FliRealObjHdl : public FliValueObjHdl {
   public:
     FliRealObjHdl(GpiImplInterface *impl, void *hdl, gpi_objtype_t objtype,
                   bool is_const, int acc_type, int acc_full_type, bool is_var,
                   mtiTypeIdT valType, mtiTypeKindT typeKind)
@@ -308,15 +320,16 @@
     }
 
     double get_signal_value_real() override;
 
     using FliValueObjHdl::set_signal_value;
     int set_signal_value(double value, gpi_set_action_t action) override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 
   private:
     double *m_mti_buff = nullptr;
 };
 
 class FliStringObjHdl : public FliValueObjHdl {
   public:
@@ -332,15 +345,16 @@
 
     const char *get_signal_value_str() override;
 
     using FliValueObjHdl::set_signal_value;
     int set_signal_value_str(std::string &value,
                              gpi_set_action_t action) override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 
   private:
     char *m_mti_buff = nullptr;
 };
 
 /** Maintains a cache of FliTimedCbHdl objects which can be reused.
  *
@@ -403,36 +417,40 @@
     void sim_end() override;
     void get_sim_time(uint32_t *high, uint32_t *low) override;
     void get_sim_precision(int32_t *precision) override;
     const char *get_simulator_product() override;
     const char *get_simulator_version() override;
 
     /* Hierachy related */
-    GpiObjHdl *native_check_create(std::string &name,
+    GpiObjHdl *native_check_create(const std::string &name,
                                    GpiObjHdl *parent) override;
     GpiObjHdl *native_check_create(int32_t index, GpiObjHdl *parent) override;
     GpiObjHdl *native_check_create(void *raw_hdl, GpiObjHdl *paret) override;
     GpiObjHdl *get_root_handle(const char *name) override;
     GpiIterator *iterate_handle(GpiObjHdl *obj_hdl,
                                 gpi_iterator_sel_t type) override;
 
     /* Callback related, these may (will) return the same handle*/
-    GpiCbHdl *register_timed_callback(uint64_t time) override;
-    GpiCbHdl *register_readonly_callback() override;
-    GpiCbHdl *register_nexttime_callback() override;
-    GpiCbHdl *register_readwrite_callback() override;
+    GpiCbHdl *register_timed_callback(uint64_t time, int (*function)(void *),
+                                      void *cb_data) override;
+    GpiCbHdl *register_readonly_callback(int (*function)(void *),
+                                         void *cb_data) override;
+    GpiCbHdl *register_nexttime_callback(int (*function)(void *),
+                                         void *cb_data) override;
+    GpiCbHdl *register_readwrite_callback(int (*function)(void *),
+                                          void *cb_data) override;
     int deregister_callback(GpiCbHdl *obj_hdl) override;
 
     /* Method to provide strings from operation types */
     const char *reason_to_string(int reason) override;
 
     /* Method to provide strings from operation types */
-    GpiObjHdl *create_gpi_obj_from_handle(void *hdl, std::string &name,
-                                          std::string &fq_name, int accType,
-                                          int accFullType);
+    GpiObjHdl *create_gpi_obj_from_handle(void *hdl, const std::string &name,
+                                          const std::string &fq_name,
+                                          int accType, int accFullType);
 
   private:
     bool isValueConst(int kind);
     bool isValueLogic(mtiTypeIdT type);
     bool isValueChar(mtiTypeIdT type);
     bool isValueBoolean(mtiTypeIdT type);
     bool isTypeValue(int type);
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/fli/FliObjHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliObjHdl.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 #include "FliImpl.h"
 #include "_vendor/fli/acc_vhdl.h"
 
 using std::abs;
 using std::to_string;
 
-GpiCbHdl *FliSignalObjHdl::value_change_cb(int edge) {
+GpiCbHdl *FliSignalObjHdl::register_value_change_callback(
+    int edge, int (*function)(void *), void *cb_data) {
     FliSignalCbHdl *cb = NULL;
 
     if (m_is_var) {
         return NULL;
     }
 
     switch (edge) {
@@ -56,19 +57,19 @@
         default:
             return NULL;
     }
 
     if (cb->arm_callback()) {
         return NULL;
     }
-
+    cb->set_user_data(function, cb_data);
     return (GpiCbHdl *)cb;
 }
 
-int FliObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliObjHdl::initialise(const std::string &name, const std::string &fq_name) {
     bool is_signal =
         (get_acc_type() == accSignal || get_acc_full_type() == accAliasSignal);
     mtiTypeIdT typeId;
     char *str;
 
     switch (get_type()) {
         case GPI_STRUCTURE:
@@ -97,19 +98,21 @@
 
     str = mti_GetRegionSourceName(get_handle<mtiRegionIdT>());
     if (str != NULL) m_definition_file = str;
 
     return GpiObjHdl::initialise(name, fq_name);
 }
 
-int FliSignalObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliSignalObjHdl::initialise(const std::string &name,
+                                const std::string &fq_name) {
     return GpiObjHdl::initialise(name, fq_name);
 }
 
-int FliValueObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliValueObjHdl::initialise(const std::string &name,
+                               const std::string &fq_name) {
     if (get_type() == GPI_ARRAY) {
         m_range_left = mti_TickLeft(m_val_type);
         m_range_right = mti_TickRight(m_val_type);
         m_num_elems = mti_TickLength(m_val_type);
         m_indexable = true;
     }
 
@@ -201,15 +204,16 @@
 
     if (idx < 0 || idx >= m_num_elems)
         return NULL;
     else
         return m_sub_hdls[idx];
 }
 
-int FliEnumObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliEnumObjHdl::initialise(const std::string &name,
+                              const std::string &fq_name) {
     m_num_elems = 1;
     m_value_enum = mti_GetEnumValues(m_val_type);
     m_num_enum = mti_TickLength(m_val_type);
 
     return FliValueObjHdl::initialise(name, fq_name);
 }
 
@@ -273,15 +277,16 @@
             default:
                 LOG_ERROR("Unknown set value action (%d)", action);
                 return -1;
         }
     }
 }
 
-int FliLogicObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliLogicObjHdl::initialise(const std::string &name,
+                               const std::string &fq_name) {
     switch (m_fli_type) {
         case MTI_TYPE_ENUM:
             m_num_elems = 1;
             m_value_enum = mti_GetEnumValues(m_val_type);
             m_num_enum = mti_TickLength(m_val_type);
             break;
         case MTI_TYPE_ARRAY: {
@@ -546,15 +551,16 @@
                     LOG_ERROR("Unknown set value action (%d)", action);
                     return -1;
             }
         }
     }
 }
 
-int FliIntObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliIntObjHdl::initialise(const std::string &name,
+                             const std::string &fq_name) {
     m_num_elems = 1;
 
     m_val_buff = new char[33];  // Integers are always 32-bits
     m_val_buff[m_num_elems] = '\0';
 
     return FliValueObjHdl::initialise(name, fq_name);
 }
@@ -631,15 +637,16 @@
             default:
                 LOG_ERROR("Unknown set value action (%d)", action);
                 return -1;
         }
     }
 }
 
-int FliRealObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliRealObjHdl::initialise(const std::string &name,
+                              const std::string &fq_name) {
     m_num_elems = 1;
 
     m_mti_buff = new double;
 
     return FliValueObjHdl::initialise(name, fq_name);
 }
 
@@ -693,15 +700,16 @@
             default:
                 LOG_ERROR("Unknown set value action (%d)", action);
                 return -1;
         }
     }
 }
 
-int FliStringObjHdl::initialise(std::string &name, std::string &fq_name) {
+int FliStringObjHdl::initialise(const std::string &name,
+                                const std::string &fq_name) {
     m_range_left = mti_TickLeft(m_val_type);
     m_range_right = mti_TickRight(m_val_type);
     m_num_elems = mti_TickLength(m_val_type);
     m_indexable = true;
 
     m_mti_buff = new char[m_num_elems];
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/gpi/GpiCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCbHdl.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -66,58 +66,43 @@
 const std::string &GpiObjHdl::get_name() { return m_name; }
 
 /* Genertic base clss implementations */
 bool GpiHdl::is_this_impl(GpiImplInterface *impl) {
     return impl == this->m_impl;
 }
 
-int GpiObjHdl::initialise(std::string &name, std::string &fq_name) {
+int GpiObjHdl::initialise(const std::string &name, const std::string &fq_name) {
     m_name = name;
     m_fullname = fq_name;
     return 0;
 }
 
-int GpiCbHdl::run_callback() {
-    LOG_TRACE("Generic run_callback");
-    this->gpi_function(m_cb_data);
-    LOG_TRACE("Generic run_callback done");
-    return 0;
-}
+void GpiCbHdl::set_call_state(gpi_cb_state_e new_state) { m_state = new_state; }
 
-int GpiCbHdl::cleanup_callback() {
-    LOG_WARN("Generic cleanup_handler");
-    return 0;
-}
+gpi_cb_state_e GpiCbHdl::get_call_state() { return m_state; }
+
+GpiCbHdl::~GpiCbHdl() {}
 
-int GpiCbHdl::arm_callback() {
-    LOG_WARN("Generic arm_callback");
+int GpiCommonCbHdl::run_callback() {
+    this->gpi_function(m_cb_data);
     return 0;
 }
 
-int GpiCbHdl::set_user_data(int (*gpi_function)(const void *),
-                            const void *data) {
+int GpiCommonCbHdl::set_user_data(int (*gpi_function)(void *), void *data) {
     if (!gpi_function) {
         LOG_ERROR("gpi_function to set_user_data is NULL");
     }
     this->gpi_function = gpi_function;
     this->m_cb_data = data;
     return 0;
 }
 
-const void *GpiCbHdl::get_user_data() { return m_cb_data; }
-
-void GpiCbHdl::set_call_state(gpi_cb_state_e new_state) { m_state = new_state; }
-
-gpi_cb_state_e GpiCbHdl::get_call_state() { return m_state; }
-
-GpiCbHdl::~GpiCbHdl() {}
-
 GpiValueCbHdl::GpiValueCbHdl(GpiImplInterface *impl, GpiSignalObjHdl *signal,
                              int edge)
-    : GpiCbHdl(impl), m_signal(signal) {
+    : GpiCbHdl(impl), GpiCommonCbHdl(impl), m_signal(signal) {
     if (edge == (GPI_RISING | GPI_FALLING))
         required_value = "X";
     else if (edge & GPI_RISING)
         required_value = "1";
     else if (edge & GPI_FALLING)
         required_value = "0";
 }
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/gpi/GpiCommon.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCommon.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 bool gpi_has_registered_impl() { return registered_impls.size() > 0; }
 
 void gpi_embed_init(int argc, char const *const *argv) {
     if (embed_sim_init(argc, argv)) gpi_embed_end();
 }
 
 void gpi_embed_end() {
-    embed_sim_event(SIM_FAIL, "Simulator shutdown prematurely");
+    embed_sim_event("Simulator shut down prematurely");
     sim_ending = true;
 }
 
 void gpi_sim_end() {
     registered_impls[0]->sim_end();
     sim_ending = true;
 }
@@ -253,15 +253,16 @@
         return CHECK_AND_STORE(hdl);
     else {
         LOG_ERROR("No root handle found");
         return hdl;
     }
 }
 
-static GpiObjHdl *gpi_get_handle_by_name_(GpiObjHdl *parent, std::string name,
+static GpiObjHdl *gpi_get_handle_by_name_(GpiObjHdl *parent,
+                                          const std::string &name,
                                           GpiImplInterface *skip_impl) {
     LOG_DEBUG("Searching for %s", name.c_str());
 
     // check parent impl *first* if it's not skipped
     if (!skip_impl || (skip_impl != parent->m_impl)) {
         auto hdl = parent->m_impl->native_check_create(name, parent);
         if (hdl) {
@@ -508,84 +509,84 @@
     return obj_hdl->get_range_left();
 }
 
 int gpi_get_range_right(gpi_sim_hdl obj_hdl) {
     return obj_hdl->get_range_right();
 }
 
-gpi_cb_hdl gpi_register_value_change_callback(int (*gpi_function)(const void *),
+gpi_cb_hdl gpi_register_value_change_callback(int (*gpi_function)(void *),
                                               void *gpi_cb_data,
                                               gpi_sim_hdl sig_hdl, int edge) {
     GpiSignalObjHdl *signal_hdl = static_cast<GpiSignalObjHdl *>(sig_hdl);
 
     /* Do something based on int & GPI_RISING | GPI_FALLING */
-    GpiCbHdl *gpi_hdl = signal_hdl->value_change_cb(edge);
+    GpiCbHdl *gpi_hdl = signal_hdl->register_value_change_callback(
+        edge, gpi_function, gpi_cb_data);
     if (!gpi_hdl) {
         LOG_ERROR("Failed to register a value change callback");
         return NULL;
+    } else {
+        return gpi_hdl;
     }
-
-    gpi_hdl->set_user_data(gpi_function, gpi_cb_data);
-    return gpi_hdl;
 }
 
-/* It should not matter which implementation we use for this so just pick the
-   first one */
-gpi_cb_hdl gpi_register_timed_callback(int (*gpi_function)(const void *),
+gpi_cb_hdl gpi_register_timed_callback(int (*gpi_function)(void *),
                                        void *gpi_cb_data, uint64_t time) {
-    GpiCbHdl *gpi_hdl = registered_impls[0]->register_timed_callback(time);
+    // It should not matter which implementation we use for this so just pick
+    // the first one
+    GpiCbHdl *gpi_hdl = registered_impls[0]->register_timed_callback(
+        time, gpi_function, gpi_cb_data);
     if (!gpi_hdl) {
         LOG_ERROR("Failed to register a timed callback");
         return NULL;
+    } else {
+        return gpi_hdl;
     }
-
-    gpi_hdl->set_user_data(gpi_function, gpi_cb_data);
-    return gpi_hdl;
 }
 
-/* It should not matter which implementation we use for this so just pick the
-   first one
-*/
-gpi_cb_hdl gpi_register_readonly_callback(int (*gpi_function)(const void *),
+gpi_cb_hdl gpi_register_readonly_callback(int (*gpi_function)(void *),
                                           void *gpi_cb_data) {
-    GpiCbHdl *gpi_hdl = registered_impls[0]->register_readonly_callback();
+    // It should not matter which implementation we use for this so just pick
+    // the first one
+    GpiCbHdl *gpi_hdl = registered_impls[0]->register_readonly_callback(
+        gpi_function, gpi_cb_data);
     if (!gpi_hdl) {
         LOG_ERROR("Failed to register a readonly callback");
         return NULL;
+    } else {
+        return gpi_hdl;
     }
-
-    gpi_hdl->set_user_data(gpi_function, gpi_cb_data);
-    return gpi_hdl;
 }
 
-gpi_cb_hdl gpi_register_nexttime_callback(int (*gpi_function)(const void *),
+gpi_cb_hdl gpi_register_nexttime_callback(int (*gpi_function)(void *),
                                           void *gpi_cb_data) {
-    GpiCbHdl *gpi_hdl = registered_impls[0]->register_nexttime_callback();
+    // It should not matter which implementation we use for this so just pick
+    // the first one
+    GpiCbHdl *gpi_hdl = registered_impls[0]->register_nexttime_callback(
+        gpi_function, gpi_cb_data);
     if (!gpi_hdl) {
         LOG_ERROR("Failed to register a nexttime callback");
         return NULL;
+    } else {
+        return gpi_hdl;
     }
-
-    gpi_hdl->set_user_data(gpi_function, gpi_cb_data);
-    return gpi_hdl;
 }
 
-/* It should not matter which implementation we use for this so just pick the
-   first one
-*/
-gpi_cb_hdl gpi_register_readwrite_callback(int (*gpi_function)(const void *),
+gpi_cb_hdl gpi_register_readwrite_callback(int (*gpi_function)(void *),
                                            void *gpi_cb_data) {
-    GpiCbHdl *gpi_hdl = registered_impls[0]->register_readwrite_callback();
+    // It should not matter which implementation we use for this so just pick
+    // the first one
+    GpiCbHdl *gpi_hdl = registered_impls[0]->register_readwrite_callback(
+        gpi_function, gpi_cb_data);
     if (!gpi_hdl) {
         LOG_ERROR("Failed to register a readwrite callback");
         return NULL;
+    } else {
+        return gpi_hdl;
     }
-
-    gpi_hdl->set_user_data(gpi_function, gpi_cb_data);
-    return gpi_hdl;
 }
 
 void gpi_deregister_callback(gpi_cb_hdl cb_hdl) {
     cb_hdl->m_impl->deregister_callback(cb_hdl);
 }
 
 const char *GpiImplInterface::get_name_c() { return m_name.c_str(); }
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/gpi/gpi_priv.h` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi/gpi_priv.h`

 * *Files 7% similar despite different names*

```diff
@@ -114,15 +114,16 @@
         return m_definition_name.c_str();
     };
     virtual const char *get_definition_file() {
         return m_definition_file.c_str();
     };
 
     bool is_native_impl(GpiImplInterface *impl);
-    virtual int initialise(std::string &name, std::string &full_name);
+    virtual int initialise(const std::string &name,
+                           const std::string &full_name);
 
   protected:
     int m_num_elems = 0;
     bool m_indexable = false;
     int m_range_left = -1;
     int m_range_right = -1;
     std::string m_name = "unknown";
@@ -160,48 +161,53 @@
                                      gpi_set_action_t action) = 0;
     virtual int set_signal_value_binstr(std::string &value,
                                         gpi_set_action_t action) = 0;
     // virtual GpiCbHdl monitor_value(bool rising_edge) = 0; this was for the
     // triggers
     // but the explicit ones are probably better
 
-    virtual GpiCbHdl *value_change_cb(int edge) = 0;
+    virtual GpiCbHdl *register_value_change_callback(
+        int edge, int (*gpi_function)(void *), void *gpi_cb_data) = 0;
 };
 
 /* GPI Callback handle */
 // To set a callback it needs the signal to do this on,
 // vpiHandle/vhpiHandleT for instance. The
 class GPI_EXPORT GpiCbHdl : public GpiHdl {
   public:
     GpiCbHdl(GpiImplInterface *impl) : GpiHdl(impl) {}
 
     // Pure virtual functions for derived classes
     virtual int arm_callback() = 0;  // Register with simulator
-    virtual int run_callback();      // Entry point from simulator
+    virtual int run_callback() = 0;  // Entry point from simulator
     virtual int
     cleanup_callback() = 0;  // Cleanup the callback, arm can be called after
 
-    // Set the data to be used for run callback, separate to arm_callback so
-    // data can be re-used
-    int set_user_data(int (*gpi_function)(const void *), const void *data);
-    const void *get_user_data();
-
     void set_call_state(gpi_cb_state_e new_state);
     gpi_cb_state_e get_call_state();
 
     virtual ~GpiCbHdl();
 
   protected:
-    int (*gpi_function)(const void *) = nullptr;  // GPI function to callback
-    const void *m_cb_data = nullptr;  // GPI data supplied to "gpi_function"
     gpi_cb_state_e m_state =
         GPI_FREE;  // GPI state of the callback through its cycle
 };
 
-class GPI_EXPORT GpiValueCbHdl : public virtual GpiCbHdl {
+class GPI_EXPORT GpiCommonCbHdl : public virtual GpiCbHdl {
+  public:
+    GpiCommonCbHdl(GpiImplInterface *impl) : GpiCbHdl(impl) {}
+    int run_callback() override;
+    int set_user_data(int (*function)(void *), void *cb_data);
+
+  protected:
+    int (*gpi_function)(void *) = nullptr;  // GPI function to callback
+    void *m_cb_data = nullptr;  // GPI data supplied to "gpi_function"
+};
+
+class GPI_EXPORT GpiValueCbHdl : public virtual GpiCommonCbHdl {
   public:
     GpiValueCbHdl(GpiImplInterface *impl, GpiSignalObjHdl *signal, int edge);
     int run_callback() override;
 
   protected:
     std::string required_value;
     GpiSignalObjHdl *m_signal;
@@ -244,29 +250,34 @@
     virtual void sim_end() = 0;
     virtual void get_sim_time(uint32_t *high, uint32_t *low) = 0;
     virtual void get_sim_precision(int32_t *precision) = 0;
     virtual const char *get_simulator_product() = 0;
     virtual const char *get_simulator_version() = 0;
 
     /* Hierarchy related */
-    virtual GpiObjHdl *native_check_create(std::string &name,
+    virtual GpiObjHdl *native_check_create(const std::string &name,
                                            GpiObjHdl *parent) = 0;
     virtual GpiObjHdl *native_check_create(int32_t index,
                                            GpiObjHdl *parent) = 0;
     virtual GpiObjHdl *native_check_create(void *raw_hdl,
                                            GpiObjHdl *parent) = 0;
     virtual GpiObjHdl *get_root_handle(const char *name) = 0;
     virtual GpiIterator *iterate_handle(GpiObjHdl *obj_hdl,
                                         gpi_iterator_sel_t type) = 0;
 
     /* Callback related, these may (will) return the same handle */
-    virtual GpiCbHdl *register_timed_callback(uint64_t time) = 0;
-    virtual GpiCbHdl *register_readonly_callback() = 0;
-    virtual GpiCbHdl *register_nexttime_callback() = 0;
-    virtual GpiCbHdl *register_readwrite_callback() = 0;
+    virtual GpiCbHdl *register_timed_callback(uint64_t time,
+                                              int (*gpi_function)(void *),
+                                              void *gpi_cb_data) = 0;
+    virtual GpiCbHdl *register_readonly_callback(int (*gpi_function)(void *),
+                                                 void *gpi_cb_data) = 0;
+    virtual GpiCbHdl *register_nexttime_callback(int (*gpi_function)(void *),
+                                                 void *gpi_cb_data) = 0;
+    virtual GpiCbHdl *register_readwrite_callback(int (*gpi_function)(void *),
+                                                  void *gpi_cb_data) = 0;
     virtual int deregister_callback(GpiCbHdl *obj_hdl) = 0;
 
     /* Method to provide strings from operation types */
     virtual const char *reason_to_string(int reason) = 0;
 
   private:
     std::string m_name;
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/gpi_log/gpi_logging.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi_log/gpi_logging.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/lib/simulator/simulatormodule.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/simulator/simulatormodule.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 PyTypeObject gpi_hdl_Object<gpi_sim_hdl>::py_type;
 template <>
 PyTypeObject gpi_hdl_Object<gpi_iterator_hdl>::py_type;
 template <>
 PyTypeObject gpi_hdl_Object<gpi_cb_hdl>::py_type;
 }  // namespace
 
-typedef int (*gpi_function_t)(const void *);
+typedef int (*gpi_function_t)(void *);
 
 PyGILState_STATE TAKE_GIL(void) {
     PyGILState_STATE state = PyGILState_Ensure();
     takes++;
     return state;
 }
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/utils/cocotb_utils.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/utils/cocotb_utils.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/lib/verilator/verilator.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/verilator/verilator.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -84,42 +84,46 @@
         // These can modify signal values
         settle_value_callbacks();
 
         // We must evaluate whole design until we process all 'events'
         bool again = true;
         while (again) {
             // Evaluate design
-            top->eval();
+            top->eval_step();
 
             // Call Value Change callbacks triggered by eval()
             // These can modify signal values
             again = settle_value_callbacks();
 
             // Call registered ReadWrite callbacks
             again |= VerilatedVpi::callCbs(cbReadWriteSynch);
 
             // Call Value Change callbacks triggered by ReadWrite callbacks
             // These can modify signal values
             again |= settle_value_callbacks();
         }
+        top->eval_end_step();
 
         // Call ReadOnly callbacks
         VerilatedVpi::callCbs(cbReadOnlySynch);
 
 #if VM_TRACE
         tfp->dump(main_time);
 #endif
         // cocotb controls the clock inputs using cbAfterDelay so
         // skip ahead to the next registered callback
-        vluint64_t next_time = VerilatedVpi::cbNextDeadline();
+        const vluint64_t NO_TOP_EVENTS_PENDING = static_cast<vluint64_t>(~0ULL);
+        vluint64_t next_time_cocotb = VerilatedVpi::cbNextDeadline();
+        vluint64_t next_time_timing =
+            top->eventsPending() ? top->nextTimeSlot() : NO_TOP_EVENTS_PENDING;
+        vluint64_t next_time = std::min(next_time_cocotb, next_time_timing);
 
         // If there are no more cbAfterDelay callbacks,
         // the next deadline is max value, so end the simulation now
-        if (next_time == static_cast<vluint64_t>(~0ULL)) {
-            vl_finish(__FILE__, __LINE__, "");
+        if (next_time == NO_TOP_EVENTS_PENDING) {
             break;
         } else {
             main_time = next_time;
         }
 
         // Call registered NextSimTime
         // It should be called in simulation cycle before everything else
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/vhpi/VhpiCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiCbHdl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 if (curr_idx == dim) {
                     vhpi_release_handle(it);
                     vhpiIntT l_rng = vhpi_get(vhpiLeftBoundP, constraint);
                     vhpiIntT r_rng = vhpi_get(vhpiRightBoundP, constraint);
 #ifdef IUS
                     if (l_rng != UNCONSTRAINED && r_rng != UNCONSTRAINED) {
 #else
-                    if (vhpi_get(vhpiIsUnconstrainedP, constraint)) {
+                    if (!vhpi_get(vhpiIsUnconstrainedP, constraint)) {
 #endif
                         error = false;
                         *left = static_cast<int>(l_rng);
                         *right = static_cast<int>(r_rng);
                     }
                     break;
                 }
@@ -170,15 +170,16 @@
             break;
         default:
             assert(0);
     }
     return put_value_mode;
 }
 
-int VhpiArrayObjHdl::initialise(std::string &name, std::string &fq_name) {
+int VhpiArrayObjHdl::initialise(const std::string &name,
+                                const std::string &fq_name) {
     vhpiHandleT handle = GpiObjHdl::get_handle<vhpiHandleT>();
 
     m_indexable = true;
 
     vhpiHandleT type = vhpi_handle(vhpiBaseType, handle);
 
     if (type == NULL) {
@@ -232,15 +233,16 @@
     } else {
         m_num_elems = m_range_right - m_range_left + 1;
     }
 
     return GpiObjHdl::initialise(name, fq_name);
 }
 
-int VhpiObjHdl::initialise(std::string &name, std::string &fq_name) {
+int VhpiObjHdl::initialise(const std::string &name,
+                           const std::string &fq_name) {
     vhpiHandleT handle = GpiObjHdl::get_handle<vhpiHandleT>();
     if (handle != NULL) {
         vhpiHandleT du_handle = vhpi_handle(vhpiDesignUnit, handle);
         if (du_handle != NULL) {
             vhpiHandleT pu_handle = vhpi_handle(vhpiPrimaryUnit, du_handle);
             if (pu_handle != NULL) {
                 const char *str;
@@ -252,15 +254,16 @@
             }
         }
     }
 
     return GpiObjHdl::initialise(name, fq_name);
 }
 
-int VhpiSignalObjHdl::initialise(std::string &name, std::string &fq_name) {
+int VhpiSignalObjHdl::initialise(const std::string &name,
+                                 const std::string &fq_name) {
     // Determine the type of object, either scalar or vector
     m_value.format = vhpiObjTypeVal;
     m_value.bufSize = 0;
     m_value.value.str = NULL;
     m_value.numElems = 0;
     /* We also alloc a second value member for use with read string operations
      */
@@ -326,15 +329,16 @@
         m_binvalue.bufSize = static_cast<bufSize_type>(bufSize);
         m_binvalue.value.str = new vhpiCharT[bufSize];
     }
 
     return GpiObjHdl::initialise(name, fq_name);
 }
 
-int VhpiLogicSignalObjHdl::initialise(std::string &name, std::string &fq_name) {
+int VhpiLogicSignalObjHdl::initialise(const std::string &name,
+                                      const std::string &fq_name) {
     // Determine the type of object, either scalar or vector
     m_value.format = vhpiLogicVal;
     m_value.bufSize = 0;
     m_value.value.str = NULL;
     m_value.numElems = 0;
     /* We also alloc a second value member for use with read string operations
      */
@@ -805,15 +809,16 @@
         check_vhpi_error();
         LOG_ERROR("VHPI: Failed to get value of type long");
     }
 
     return static_cast<int32_t>(value.value.intg);
 }
 
-GpiCbHdl *VhpiSignalObjHdl::value_change_cb(int edge) {
+GpiCbHdl *VhpiSignalObjHdl::register_value_change_callback(
+    int edge, int (*function)(void *), void *cb_data) {
     VhpiValueCbHdl *cb = NULL;
 
     switch (edge) {
         case 1:
             cb = &m_rising_cb;
             break;
         case 2:
@@ -822,24 +827,28 @@
         case 3:
             cb = &m_either_cb;
             break;
         default:
             return NULL;
     }
 
+    cb->set_user_data(function, cb_data);
     if (cb->arm_callback()) {
         return NULL;
     }
 
     return cb;
 }
 
 VhpiValueCbHdl::VhpiValueCbHdl(GpiImplInterface *impl, VhpiSignalObjHdl *sig,
                                int edge)
-    : GpiCbHdl(impl), VhpiCbHdl(impl), GpiValueCbHdl(impl, sig, edge) {
+    : GpiCbHdl(impl),
+      GpiCommonCbHdl(impl),
+      VhpiCbHdl(impl),
+      GpiValueCbHdl(impl, sig, edge) {
     cb_data.reason = vhpiCbValueChange;
     cb_data.time = &vhpi_time;
     cb_data.obj = m_signal->get_handle<vhpiHandleT>();
 }
 
 VhpiStartupCbHdl::VhpiStartupCbHdl(GpiImplInterface *impl)
     : GpiCbHdl(impl), VhpiCbHdl(impl) {
@@ -861,15 +870,14 @@
         argv_iter = vhpi_iterator(vhpiArgvs, tool);
         if (argv_iter) {
             while ((argv_hdl = vhpi_scan(argv_iter))) {
                 tool_argv[i] = const_cast<char *>(static_cast<const char *>(
                     vhpi_get_str(vhpiStrValP, argv_hdl)));
                 i++;
             }
-            vhpi_release_handle(argv_iter);
         }
 
         vhpi_release_handle(tool);
     }
 
     gpi_embed_init(tool_argc, tool_argv);
     delete[] tool_argv;
@@ -885,15 +893,15 @@
 int VhpiShutdownCbHdl::run_callback() {
     set_call_state(GPI_DELETE);
     gpi_embed_end();
     return 0;
 }
 
 VhpiTimedCbHdl::VhpiTimedCbHdl(GpiImplInterface *impl, uint64_t time)
-    : GpiCbHdl(impl), VhpiCbHdl(impl) {
+    : GpiCbHdl(impl), VhpiCommonCbHdl(impl) {
     vhpi_time.high = (uint32_t)(time >> 32);
     vhpi_time.low = (uint32_t)(time);
 
     cb_data.reason = vhpiCbAfterDelay;
     cb_data.time = &vhpi_time;
 }
 
@@ -903,28 +911,28 @@
     vhpi_remove_cb(get_handle<vhpiHandleT>());
 
     m_obj_hdl = NULL;
     m_state = GPI_FREE;
     return 1;
 }
 
-VhpiReadwriteCbHdl::VhpiReadwriteCbHdl(GpiImplInterface *impl)
-    : GpiCbHdl(impl), VhpiCbHdl(impl) {
+VhpiReadWriteCbHdl::VhpiReadWriteCbHdl(GpiImplInterface *impl)
+    : GpiCbHdl(impl), VhpiCommonCbHdl(impl) {
     cb_data.reason = vhpiCbRepLastKnownDeltaCycle;
     cb_data.time = &vhpi_time;
 }
 
 VhpiReadOnlyCbHdl::VhpiReadOnlyCbHdl(GpiImplInterface *impl)
-    : GpiCbHdl(impl), VhpiCbHdl(impl) {
+    : GpiCbHdl(impl), VhpiCommonCbHdl(impl) {
     cb_data.reason = vhpiCbRepEndOfTimeStep;
     cb_data.time = &vhpi_time;
 }
 
 VhpiNextPhaseCbHdl::VhpiNextPhaseCbHdl(GpiImplInterface *impl)
-    : GpiCbHdl(impl), VhpiCbHdl(impl) {
+    : GpiCbHdl(impl), VhpiCommonCbHdl(impl) {
     cb_data.reason = vhpiCbRepNextTimeStep;
     cb_data.time = &vhpi_time;
 }
 
 decltype(VhpiIterator::iterate_over) VhpiIterator::iterate_over = [] {
     /* for reused lists */
     std::initializer_list<vhpiOneToManyT> root_options = {
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/vhpi/VhpiImpl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -262,16 +262,16 @@
         }
     }
 
     return false;
 }
 
 GpiObjHdl *VhpiImpl::create_gpi_obj_from_handle(vhpiHandleT new_hdl,
-                                                std::string &name,
-                                                std::string &fq_name) {
+                                                const std::string &name,
+                                                const std::string &fq_name) {
     vhpiIntT type;
     gpi_objtype_t gpi_type;
     GpiObjHdl *new_obj = NULL;
 
     if (vhpiVerilog == (type = vhpi_get(vhpiKindP, new_hdl))) {
         LOG_DEBUG("VHPI: vhpiVerilog returned from vhpi_get(vhpiType, ...)")
         return NULL;
@@ -311,23 +311,29 @@
                 LOG_DEBUG("VHPI: Detected a MULTI-DIMENSIONAL ARRAY type %s",
                           fq_name.c_str());
                 gpi_type = GPI_ARRAY;
             } else {
                 vhpiHandleT elem_base_type_hdl = NULL;
                 vhpiIntT elem_base_type = 0;
 
-                /* vhpiElemSubtype is deprecated.  Should be using vhpiElemType,
-                 * but not supported in all simulators. */
                 vhpiHandleT elem_sub_type_hdl =
-                    vhpi_handle(vhpiElemSubtype, query_hdl);
+                    vhpi_handle(vhpiElemType, query_hdl);
+                /* vhpiElemType is not supported in all simulators. */
+                if (!elem_sub_type_hdl) {
+                    elem_sub_type_hdl = vhpi_handle(vhpiElemSubtype, query_hdl);
+                }
 
                 if (elem_sub_type_hdl != NULL) {
                     elem_base_type_hdl =
                         vhpi_handle(vhpiBaseType, elem_sub_type_hdl);
-                    vhpi_release_handle(elem_sub_type_hdl);
+                    if (elem_base_type_hdl == NULL) {
+                        elem_base_type_hdl = elem_sub_type_hdl;
+                    } else {
+                        vhpi_release_handle(elem_sub_type_hdl);
+                    }
                 }
 
                 if (elem_base_type_hdl != NULL) {
                     elem_base_type = vhpi_get(vhpiKindP, elem_base_type_hdl);
                     if (elem_base_type == vhpiEnumTypeDeclK) {
                         if (is_enum_logic(elem_base_type_hdl)) {
                             LOG_DEBUG("VHPI: Detected a LOGIC VECTOR type %s",
@@ -496,15 +502,16 @@
         LOG_DEBUG("VHPI: Unable to fetch object %s", fq_name.c_str());
         return NULL;
     }
 
     return new_obj;
 }
 
-GpiObjHdl *VhpiImpl::native_check_create(std::string &name, GpiObjHdl *parent) {
+GpiObjHdl *VhpiImpl::native_check_create(const std::string &name,
+                                         GpiObjHdl *parent) {
     vhpiHandleT vhpi_hdl = parent->get_handle<vhpiHandleT>();
 
     vhpiHandleT new_hdl;
     std::string fq_name = parent->get_fullname();
     if (fq_name == ":") {
         fq_name += name;
     } else {
@@ -927,40 +934,45 @@
         default:
             LOG_WARN("VHPI: Other iterator types not implemented yet");
             break;
     }
     return new_iter;
 }
 
-GpiCbHdl *VhpiImpl::register_timed_callback(uint64_t time) {
+GpiCbHdl *VhpiImpl::register_timed_callback(uint64_t time,
+                                            int (*function)(void *),
+                                            void *cb_data) {
     VhpiTimedCbHdl *hdl = new VhpiTimedCbHdl(this, time);
 
     if (hdl->arm_callback()) {
         delete (hdl);
-        hdl = NULL;
+        return NULL;
     }
-
+    hdl->set_user_data(function, cb_data);
     return hdl;
 }
 
-GpiCbHdl *VhpiImpl::register_readwrite_callback() {
+GpiCbHdl *VhpiImpl::register_readwrite_callback(int (*function)(void *),
+                                                void *cb_data) {
     if (m_read_write.arm_callback()) return NULL;
-
+    m_read_write.set_user_data(function, cb_data);
     return &m_read_write;
 }
 
-GpiCbHdl *VhpiImpl::register_readonly_callback() {
+GpiCbHdl *VhpiImpl::register_readonly_callback(int (*function)(void *),
+                                               void *cb_data) {
     if (m_read_only.arm_callback()) return NULL;
-
+    m_read_only.set_user_data(function, cb_data);
     return &m_read_only;
 }
 
-GpiCbHdl *VhpiImpl::register_nexttime_callback() {
+GpiCbHdl *VhpiImpl::register_nexttime_callback(int (*function)(void *),
+                                               void *cb_data) {
     if (m_next_phase.arm_callback()) return NULL;
-
+    m_next_phase.set_user_data(function, cb_data);
     return &m_next_phase;
 }
 
 int VhpiImpl::deregister_callback(GpiCbHdl *gpi_hdl) {
     gpi_hdl->cleanup_callback();
     return 0;
 }
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/vhpi/VhpiImpl.h` & `cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.h`

 * *Files 5% similar despite different names*

```diff
@@ -116,26 +116,32 @@
     VhpiValueCbHdl(GpiImplInterface *impl, VhpiSignalObjHdl *sig, int edge);
     int cleanup_callback() override { return VhpiCbHdl::cleanup_callback(); }
 
   private:
     std::string initial_value;
 };
 
-class VhpiTimedCbHdl : public VhpiCbHdl {
+class VhpiCommonCbHdl : public VhpiCbHdl, public GpiCommonCbHdl {
+  public:
+    VhpiCommonCbHdl(GpiImplInterface *impl)
+        : GpiCbHdl(impl), VhpiCbHdl(impl), GpiCommonCbHdl(impl) {}
+};
+
+class VhpiTimedCbHdl : public VhpiCommonCbHdl {
   public:
     VhpiTimedCbHdl(GpiImplInterface *impl, uint64_t time);
     int cleanup_callback() override;
 };
 
-class VhpiReadOnlyCbHdl : public VhpiCbHdl {
+class VhpiReadOnlyCbHdl : public VhpiCommonCbHdl {
   public:
     VhpiReadOnlyCbHdl(GpiImplInterface *impl);
 };
 
-class VhpiNextPhaseCbHdl : public VhpiCbHdl {
+class VhpiNextPhaseCbHdl : public VhpiCommonCbHdl {
   public:
     VhpiNextPhaseCbHdl(GpiImplInterface *impl);
 };
 
 class VhpiStartupCbHdl : public VhpiCbHdl {
   public:
     VhpiStartupCbHdl(GpiImplInterface *impl);
@@ -154,36 +160,38 @@
     int cleanup_callback() override {
         /* Too many simulators get upset with this so we override to do nothing
          */
         return 0;
     }
 };
 
-class VhpiReadwriteCbHdl : public VhpiCbHdl {
+class VhpiReadWriteCbHdl : public VhpiCommonCbHdl {
   public:
-    VhpiReadwriteCbHdl(GpiImplInterface *impl);
+    VhpiReadWriteCbHdl(GpiImplInterface *impl);
 };
 
 class VhpiArrayObjHdl : public GpiObjHdl {
   public:
     VhpiArrayObjHdl(GpiImplInterface *impl, vhpiHandleT hdl,
                     gpi_objtype_t objtype)
         : GpiObjHdl(impl, hdl, objtype) {}
     ~VhpiArrayObjHdl() override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 };
 
 class VhpiObjHdl : public GpiObjHdl {
   public:
     VhpiObjHdl(GpiImplInterface *impl, vhpiHandleT hdl, gpi_objtype_t objtype)
         : GpiObjHdl(impl, hdl, objtype) {}
     ~VhpiObjHdl() override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 };
 
 class VhpiSignalObjHdl : public GpiSignalObjHdl {
   public:
     VhpiSignalObjHdl(GpiImplInterface *impl, vhpiHandleT hdl,
                      gpi_objtype_t objtype, bool is_const)
         : GpiSignalObjHdl(impl, hdl, objtype, is_const),
@@ -202,16 +210,18 @@
     int set_signal_value(double value, gpi_set_action_t action) override;
     int set_signal_value_str(std::string &value,
                              gpi_set_action_t action) override;
     int set_signal_value_binstr(std::string &value,
                                 gpi_set_action_t action) override;
 
     /* Value change callback accessor */
-    GpiCbHdl *value_change_cb(int edge) override;
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
+    GpiCbHdl *register_value_change_callback(int edge, int (*function)(void *),
+                                             void *cb_data) override;
 
   protected:
     vhpiEnumT chr2vhpi(char value);
     vhpiValueT m_value;
     vhpiValueT m_binvalue;
     VhpiValueCbHdl m_rising_cb;
     VhpiValueCbHdl m_falling_cb;
@@ -225,15 +235,16 @@
         : VhpiSignalObjHdl(impl, hdl, objtype, is_const) {}
 
     using GpiSignalObjHdl::set_signal_value;
     int set_signal_value(int32_t value, gpi_set_action_t action) override;
     int set_signal_value_binstr(std::string &value,
                                 gpi_set_action_t action) override;
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 };
 
 class VhpiIterator : public GpiIterator {
   public:
     VhpiIterator(GpiImplInterface *impl, GpiObjHdl *hdl);
 
     ~VhpiIterator() override;
@@ -267,31 +278,35 @@
 
     /* Hierachy related */
     GpiObjHdl *get_root_handle(const char *name) override;
     GpiIterator *iterate_handle(GpiObjHdl *obj_hdl,
                                 gpi_iterator_sel_t type) override;
 
     /* Callback related, these may (will) return the same handle*/
-    GpiCbHdl *register_timed_callback(uint64_t time) override;
-    GpiCbHdl *register_readonly_callback() override;
-    GpiCbHdl *register_nexttime_callback() override;
-    GpiCbHdl *register_readwrite_callback() override;
+    GpiCbHdl *register_timed_callback(uint64_t time, int (*function)(void *),
+                                      void *cb_data) override;
+    GpiCbHdl *register_readonly_callback(int (*function)(void *),
+                                         void *cb_data) override;
+    GpiCbHdl *register_nexttime_callback(int (*function)(void *),
+                                         void *cb_data) override;
+    GpiCbHdl *register_readwrite_callback(int (*function)(void *),
+                                          void *cb_data) override;
     int deregister_callback(GpiCbHdl *obj_hdl) override;
-    GpiObjHdl *native_check_create(std::string &name,
+    GpiObjHdl *native_check_create(const std::string &name,
                                    GpiObjHdl *parent) override;
     GpiObjHdl *native_check_create(int32_t index, GpiObjHdl *parent) override;
     GpiObjHdl *native_check_create(void *raw_hdl, GpiObjHdl *parent) override;
 
     const char *reason_to_string(int reason) override;
     const char *format_to_string(int format);
 
     GpiObjHdl *create_gpi_obj_from_handle(vhpiHandleT new_hdl,
-                                          std::string &name,
-                                          std::string &fq_name);
+                                          const std::string &name,
+                                          const std::string &fq_name);
 
   private:
-    VhpiReadwriteCbHdl m_read_write;
+    VhpiReadWriteCbHdl m_read_write;
     VhpiNextPhaseCbHdl m_next_phase;
     VhpiReadOnlyCbHdl m_read_only;
 };
 
 #endif /*COCOTB_VHPI_IMPL_H_  */
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/vpi/VpiCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiCbHdl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,16 @@
 
     m_obj_hdl = NULL;
     m_state = GPI_FREE;
 
     return 0;
 }
 
-int VpiArrayObjHdl::initialise(std::string &name, std::string &fq_name) {
+int VpiArrayObjHdl::initialise(const std::string &name,
+                               const std::string &fq_name) {
     vpiHandle hdl = GpiObjHdl::get_handle<vpiHandle>();
 
     m_indexable = true;
 
     int range_idx = 0;
 
     /* Need to determine if this is a pseudo-handle to be able to select the
@@ -203,26 +204,27 @@
     } else {
         m_num_elems = m_range_right - m_range_left + 1;
     }
 
     return GpiObjHdl::initialise(name, fq_name);
 }
 
-int VpiObjHdl::initialise(std::string &name, std::string &fq_name) {
+int VpiObjHdl::initialise(const std::string &name, const std::string &fq_name) {
     char *str;
     vpiHandle hdl = GpiObjHdl::get_handle<vpiHandle>();
     str = vpi_get_str(vpiDefName, hdl);
     if (str != NULL) m_definition_name = str;
     str = vpi_get_str(vpiDefFile, hdl);
     if (str != NULL) m_definition_file = str;
 
     return GpiObjHdl::initialise(name, fq_name);
 }
 
-int VpiSignalObjHdl::initialise(std::string &name, std::string &fq_name) {
+int VpiSignalObjHdl::initialise(const std::string &name,
+                                const std::string &fq_name) {
     int32_t type = vpi_get(vpiType, GpiObjHdl::get_handle<vpiHandle>());
     if ((vpiIntVar == type) || (vpiIntegerVar == type) ||
         (vpiIntegerNet == type) || (vpiRealNet == type)) {
         m_num_elems = 1;
     } else {
         m_num_elems = vpi_get(vpiSize, GpiObjHdl::get_handle<vpiHandle>());
 
@@ -409,15 +411,16 @@
     }
 
     check_vpi_error();
 
     return 0;
 }
 
-GpiCbHdl *VpiSignalObjHdl::value_change_cb(int edge) {
+GpiCbHdl *VpiSignalObjHdl::register_value_change_callback(
+    int edge, int (*function)(void *), void *cb_data) {
     VpiValueCbHdl *cb = NULL;
 
     switch (edge) {
         case 1:
             cb = &m_rising_cb;
             break;
         case 2:
@@ -426,24 +429,28 @@
         case 3:
             cb = &m_either_cb;
             break;
         default:
             return NULL;
     }
 
+    cb->set_user_data(function, cb_data);
     if (cb->arm_callback()) {
         return NULL;
     }
 
     return cb;
 }
 
 VpiValueCbHdl::VpiValueCbHdl(GpiImplInterface *impl, VpiSignalObjHdl *sig,
                              int edge)
-    : GpiCbHdl(impl), VpiCbHdl(impl), GpiValueCbHdl(impl, sig, edge) {
+    : GpiCbHdl(impl),
+      GpiCommonCbHdl(impl),
+      VpiCbHdl(impl),
+      GpiValueCbHdl(impl, sig, edge) {
     vpi_time.type = vpiSuppressTime;
     m_vpi_value.format = vpiIntVal;
 
     cb_data.reason = cbValueChange;
     cb_data.time = &vpi_time;
     cb_data.value = &m_vpi_value;
     cb_data.obj = m_signal->get_handle<vpiHandle>();
@@ -497,15 +504,15 @@
 
 int VpiShutdownCbHdl::run_callback() {
     gpi_embed_end();
     return 0;
 }
 
 VpiTimedCbHdl::VpiTimedCbHdl(GpiImplInterface *impl, uint64_t time)
-    : GpiCbHdl(impl), VpiCbHdl(impl) {
+    : GpiCbHdl(impl), VpiCommonCbHdl(impl) {
     vpi_time.high = (uint32_t)(time >> 32);
     vpi_time.low = (uint32_t)(time);
     vpi_time.type = vpiSimTime;
 
     cb_data.reason = cbAfterDelay;
 }
 
@@ -524,26 +531,26 @@
             break;
     }
     VpiCbHdl::cleanup_callback();
     /* Return one so we delete this object */
     return 1;
 }
 
-VpiReadwriteCbHdl::VpiReadwriteCbHdl(GpiImplInterface *impl)
-    : GpiCbHdl(impl), VpiCbHdl(impl) {
+VpiReadWriteCbHdl::VpiReadWriteCbHdl(GpiImplInterface *impl)
+    : GpiCbHdl(impl), VpiCommonCbHdl(impl) {
     cb_data.reason = cbReadWriteSynch;
 }
 
 VpiReadOnlyCbHdl::VpiReadOnlyCbHdl(GpiImplInterface *impl)
-    : GpiCbHdl(impl), VpiCbHdl(impl) {
+    : GpiCbHdl(impl), VpiCommonCbHdl(impl) {
     cb_data.reason = cbReadOnlySynch;
 }
 
 VpiNextPhaseCbHdl::VpiNextPhaseCbHdl(GpiImplInterface *impl)
-    : GpiCbHdl(impl), VpiCbHdl(impl) {
+    : GpiCbHdl(impl), VpiCommonCbHdl(impl) {
     cb_data.reason = cbNextSimTime;
 }
 
 decltype(VpiIterator::iterate_over) VpiIterator::iterate_over = [] {
     /* for reused lists */
 
     // vpiInstance is the base class for module, program, interface, etc.
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/vpi/VpiImpl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         case vpiIntegerVar:
         case vpiIntegerNet:
             return GPI_INTEGER;
 
         case vpiStructVar:
         case vpiStructNet:
         case vpiUnionVar:
+        case vpiUnionNet:
             return GPI_STRUCTURE;
 
         case vpiModport:
         case vpiInterface:
         case vpiModule:
         case vpiRefObj:
         case vpiPort:
@@ -168,16 +169,16 @@
             LOG_DEBUG("Unable to map vpiConst type %d onto GPI type",
                       const_type);
             return GPI_UNKNOWN;
     }
 }
 
 GpiObjHdl *VpiImpl::create_gpi_obj_from_handle(vpiHandle new_hdl,
-                                               std::string &name,
-                                               std::string &fq_name) {
+                                               const std::string &name,
+                                               const std::string &fq_name) {
     int32_t type;
     GpiObjHdl *new_obj = NULL;
     if (vpiUnknown == (type = vpi_get(vpiType, new_hdl))) {
         LOG_DEBUG("vpiUnknown returned from vpi_get(vpiType, ...)")
         return NULL;
     }
 
@@ -215,14 +216,15 @@
         case vpiMemory:
         case vpiInterconnectArray:
             new_obj = new VpiArrayObjHdl(this, new_hdl, to_gpi_objtype(type));
             break;
         case vpiStructVar:
         case vpiStructNet:
         case vpiUnionVar:
+        case vpiUnionNet:
             new_obj = new VpiObjHdl(this, new_hdl, to_gpi_objtype(type));
             break;
         case vpiModule:
         case vpiInterface:
         case vpiModport:
         case vpiRefObj:
         case vpiPort:
@@ -288,15 +290,16 @@
         vpi_free_object(new_hdl);
         LOG_DEBUG("Unable to fetch object %s", fq_name.c_str());
         return NULL;
     }
     return new_obj;
 }
 
-GpiObjHdl *VpiImpl::native_check_create(std::string &name, GpiObjHdl *parent) {
+GpiObjHdl *VpiImpl::native_check_create(const std::string &name,
+                                        GpiObjHdl *parent) {
     vpiHandle new_hdl;
     const vpiHandle parent_hdl = parent->get_handle<vpiHandle>();
     std::string fq_name = parent->get_fullname() + "." + name;
 
     new_hdl = vpi_handle_by_name(const_cast<char *>(fq_name.c_str()), NULL);
 
 #ifdef ICARUS
@@ -573,40 +576,45 @@
         default:
             LOG_WARN("Other iterator types not implemented yet");
             break;
     }
     return new_iter;
 }
 
-GpiCbHdl *VpiImpl::register_timed_callback(uint64_t time) {
+GpiCbHdl *VpiImpl::register_timed_callback(uint64_t time,
+                                           int (*function)(void *),
+                                           void *cb_data) {
     VpiTimedCbHdl *hdl = new VpiTimedCbHdl(this, time);
 
     if (hdl->arm_callback()) {
         delete (hdl);
-        hdl = NULL;
+        return NULL;
     }
-
+    hdl->set_user_data(function, cb_data);
     return hdl;
 }
 
-GpiCbHdl *VpiImpl::register_readwrite_callback() {
+GpiCbHdl *VpiImpl::register_readwrite_callback(int (*function)(void *),
+                                               void *cb_data) {
     if (m_read_write.arm_callback()) return NULL;
-
+    m_read_write.set_user_data(function, cb_data);
     return &m_read_write;
 }
 
-GpiCbHdl *VpiImpl::register_readonly_callback() {
+GpiCbHdl *VpiImpl::register_readonly_callback(int (*function)(void *),
+                                              void *cb_data) {
     if (m_read_only.arm_callback()) return NULL;
-
+    m_read_only.set_user_data(function, cb_data);
     return &m_read_only;
 }
 
-GpiCbHdl *VpiImpl::register_nexttime_callback() {
+GpiCbHdl *VpiImpl::register_nexttime_callback(int (*function)(void *),
+                                              void *cb_data) {
     if (m_next_phase.arm_callback()) return NULL;
-
+    m_next_phase.set_user_data(function, cb_data);
     return &m_next_phase;
 }
 
 int VpiImpl::deregister_callback(GpiCbHdl *gpi_hdl) {
     return gpi_hdl->cleanup_callback();
 }
```

### Comparing `cocotb-1.7.2/cocotb/share/lib/vpi/VpiImpl.h` & `cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.h`

 * *Files 4% similar despite different names*

```diff
@@ -107,33 +107,39 @@
     VpiValueCbHdl(GpiImplInterface *impl, VpiSignalObjHdl *sig, int edge);
     int cleanup_callback() override;
 
   private:
     s_vpi_value m_vpi_value;
 };
 
-class VpiTimedCbHdl : public VpiCbHdl {
+class VpiCommonCbHdl : public VpiCbHdl, public GpiCommonCbHdl {
+  public:
+    VpiCommonCbHdl(GpiImplInterface *impl)
+        : GpiCbHdl(impl), VpiCbHdl(impl), GpiCommonCbHdl(impl) {}
+};
+
+class VpiTimedCbHdl : public VpiCommonCbHdl {
   public:
     VpiTimedCbHdl(GpiImplInterface *impl, uint64_t time);
     int cleanup_callback() override;
 };
 
-class VpiReadOnlyCbHdl : public VpiCbHdl {
+class VpiReadOnlyCbHdl : public VpiCommonCbHdl {
   public:
     VpiReadOnlyCbHdl(GpiImplInterface *impl);
 };
 
-class VpiNextPhaseCbHdl : public VpiCbHdl {
+class VpiNextPhaseCbHdl : public VpiCommonCbHdl {
   public:
     VpiNextPhaseCbHdl(GpiImplInterface *impl);
 };
 
-class VpiReadwriteCbHdl : public VpiCbHdl {
+class VpiReadWriteCbHdl : public VpiCommonCbHdl {
   public:
-    VpiReadwriteCbHdl(GpiImplInterface *impl);
+    VpiReadWriteCbHdl(GpiImplInterface *impl);
 };
 
 class VpiStartupCbHdl : public VpiCbHdl {
   public:
     VpiStartupCbHdl(GpiImplInterface *impl);
     int run_callback() override;
     int cleanup_callback() override {
@@ -153,23 +159,25 @@
 };
 
 class VpiArrayObjHdl : public GpiObjHdl {
   public:
     VpiArrayObjHdl(GpiImplInterface *impl, vpiHandle hdl, gpi_objtype_t objtype)
         : GpiObjHdl(impl, hdl, objtype) {}
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 };
 
 class VpiObjHdl : public GpiObjHdl {
   public:
     VpiObjHdl(GpiImplInterface *impl, vpiHandle hdl, gpi_objtype_t objtype)
         : GpiObjHdl(impl, hdl, objtype) {}
 
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
 };
 
 class VpiSignalObjHdl : public GpiSignalObjHdl {
   public:
     VpiSignalObjHdl(GpiImplInterface *impl, vpiHandle hdl,
                     gpi_objtype_t objtype, bool is_const)
         : GpiSignalObjHdl(impl, hdl, objtype, is_const),
@@ -186,16 +194,18 @@
     int set_signal_value(const double value, gpi_set_action_t action) override;
     int set_signal_value_binstr(std::string &value,
                                 gpi_set_action_t action) override;
     int set_signal_value_str(std::string &value,
                              gpi_set_action_t action) override;
 
     /* Value change callback accessor */
-    GpiCbHdl *value_change_cb(int edge) override;
-    int initialise(std::string &name, std::string &fq_name) override;
+    int initialise(const std::string &name,
+                   const std::string &fq_name) override;
+    GpiCbHdl *register_value_change_callback(int edge, int (*function)(void *),
+                                             void *cb_data) override;
 
   private:
     int set_signal_value(s_vpi_value value, gpi_set_action_t action);
 
     VpiValueCbHdl m_rising_cb;
     VpiValueCbHdl m_falling_cb;
     VpiValueCbHdl m_either_cb;
@@ -260,28 +270,33 @@
     /* Hierarchy related */
     GpiObjHdl *get_root_handle(const char *name) override;
     GpiIterator *iterate_handle(GpiObjHdl *obj_hdl,
                                 gpi_iterator_sel_t type) override;
     GpiObjHdl *next_handle(GpiIterator *iter);
 
     /* Callback related, these may (will) return the same handle*/
-    GpiCbHdl *register_timed_callback(uint64_t time) override;
-    GpiCbHdl *register_readonly_callback() override;
-    GpiCbHdl *register_nexttime_callback() override;
-    GpiCbHdl *register_readwrite_callback() override;
+    GpiCbHdl *register_timed_callback(uint64_t time, int (*function)(void *),
+                                      void *cb_data) override;
+    GpiCbHdl *register_readonly_callback(int (*function)(void *),
+                                         void *cb_data) override;
+    GpiCbHdl *register_nexttime_callback(int (*function)(void *),
+                                         void *cb_data) override;
+    GpiCbHdl *register_readwrite_callback(int (*function)(void *),
+                                          void *cb_data) override;
     int deregister_callback(GpiCbHdl *obj_hdl) override;
-    GpiObjHdl *native_check_create(std::string &name,
+    GpiObjHdl *native_check_create(const std::string &name,
                                    GpiObjHdl *parent) override;
     GpiObjHdl *native_check_create(int32_t index, GpiObjHdl *parent) override;
     GpiObjHdl *native_check_create(void *raw_hdl, GpiObjHdl *parent) override;
     const char *reason_to_string(int reason) override;
-    GpiObjHdl *create_gpi_obj_from_handle(vpiHandle new_hdl, std::string &name,
-                                          std::string &fq_name);
+    GpiObjHdl *create_gpi_obj_from_handle(vpiHandle new_hdl,
+                                          const std::string &name,
+                                          const std::string &fq_name);
 
   private:
     /* Singleton callbacks */
-    VpiReadwriteCbHdl m_read_write;
+    VpiReadWriteCbHdl m_read_write;
     VpiNextPhaseCbHdl m_next_phase;
     VpiReadOnlyCbHdl m_read_only;
 };
 
 #endif /*COCOTB_VPI_IMPL_H_  */
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/Makefile.inc` & `cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.inc`

 * *Files 5% similar despite different names*

```diff
@@ -53,29 +53,41 @@
 ifneq (, $(findstring MINGW, $(OS)))
     OS := Msys
 else ifneq (, $(findstring MSYS, $(OS)))
     OS := Msys
 endif
 export OS
 
+# Detects if Python is running in a virtual environment
+# https://docs.python.org/3/library/venv.html
+IS_VENV=$(shell $(shell cocotb-config --python-bin) -c 'import sys; print(sys.prefix != sys.base_prefix)')
+
 # this ensures we use the same python as the one cocotb was installed into
-# realpath to convert windows paths to unix paths, like cygpath -u
-PYTHON_BIN ?= $(realpath $(shell cocotb-config --python-bin))
+ifeq ($(IS_VENV),True)
+    # In a virtual environment, the Python binary may be a symlink, so it should not use realpath
+    PYTHON_BIN ?= $(shell cocotb-config --python-bin)
+else
+    # realpath to convert windows paths to unix paths, like cygpath -u
+    PYTHON_BIN ?= $(realpath $(shell cocotb-config --python-bin))
+endif
 
 include $(COCOTB_SHARE_DIR)/makefiles/Makefile.deprecations
 
 LIB_DIR=$(COCOTB_PY_DIR)/cocotb/libs
 
 PYTHON_ARCH := $(shell $(PYTHON_BIN) -c 'from platform import architecture; print(architecture()[0])')
 ifeq ($(filter $(PYTHON_ARCH),64bit 32bit),)
     $(error Unknown Python architecture: $(PYTHON_ARCH))
 endif
 
-# Set PYTHONHOME to properly populate sys.path in embedded python interpreter
-export PYTHONHOME := $(shell $(PYTHON_BIN) -c 'import sys; print(sys.prefix)')
+# Changing PYTHONHOME confuses virtual environments, so only set it when not using a venv
+ifeq ($(IS_VENV),False)
+    # Set PYTHONHOME to properly populate sys.path in embedded python interpreter
+    export PYTHONHOME := $(shell $(PYTHON_BIN) -c 'import sys; print(sys.prefix)')
+endif
 
 ifeq ($(OS),Msys)
     to_tcl_path = $(shell cygpath -m $(1) )
 else
     to_tcl_path = $(1)
 endif
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/Makefile.sim` & `cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.sim`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 Makefile-based Test Scripts
 ---------------------------
 GUI                       Set this to 1 to enable the GUI mode in the simulator
 SIM                       Selects which simulator Makefile to use
 WAVES                     Enable wave traces dump for Riviera-PRO and Questa
 VERILOG_SOURCES           A list of the Verilog source files to include
 VHDL_SOURCES              A list of the VHDL source files to include
-VHDL_SOURCES_<lib>        VHDL source files to include in *lib* (GHDL/ModelSim/Questa/Xcelium only)
-VHDL_LIB_ORDER            Compilation order of VHDL libraries (needed for ModelSim/Questa/Xcelium)
+VHDL_SOURCES_<lib>        VHDL source files to include in *lib* (GHDL/ModelSim/Questa/Xcelium/Incisive only)
+VHDL_LIB_ORDER            Compilation order of VHDL libraries (needed for ModelSim/Questa/Xcelium/Incisive)
 SIM_CMD_PREFIX            Prefix for simulation command invocations
 COMPILE_ARGS              Arguments to pass to compile stage of simulation
 SIM_ARGS                  Arguments to pass to execution of compiled simulation
 EXTRA_ARGS                Arguments for compile and execute phases
 PLUSARGS                  Plusargs to pass to the simulator
 COCOTB_HDL_TIMEUNIT       Default time unit for simulation
 COCOTB_HDL_TIMEPRECISION  Default time precision for simulation
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.activehdl` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.activehdl`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.cvc` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.cvc`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.ghdl` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ghdl`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.icarus` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.vcs`

 * *Files 12% similar despite different names*

```diff
@@ -23,70 +23,76 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ###############################################################################
 
-TOPLEVEL_LANG ?= verilog
-
 include $(shell cocotb-config --makefiles)/Makefile.inc
 
-ifneq ($(or $(filter-out $(TOPLEVEL_LANG),verilog),$(VHDL_SOURCES)),)
+ifneq ($(VHDL_SOURCES),)
 
 $(COCOTB_RESULTS_FILE):
-	@echo "Skipping simulation as only Verilog is supported on simulator=$(SIM)"
-debug: $(COCOTB_RESULTS_FILE)
+	@echo "Skipping simulation as VHDL is not supported on simulator=$(SIM)"
 clean::
 
 else
 
-CMD_BIN := iverilog
+CMD_BIN := vcs
 
-ifdef ICARUS_BIN_DIR
-    CMD := $(shell :; command -v $(ICARUS_BIN_DIR)/$(CMD_BIN) 2>/dev/null)
+ifdef VCS_BIN_DIR
+     CMD := $(shell :; command -v $(VCS_BIN_DIR)/$(CMD_BIN) 2>/dev/null)
 else
-    # auto-detect bin dir from system path
-    CMD := $(shell :; command -v $(CMD_BIN) 2>/dev/null)
+     # auto-detect bin dir from system path
+     CMD := $(shell :; command -v $(CMD_BIN) 2>/dev/null)
 endif
 
 ifeq (, $(CMD))
-    $(error Unable to locate command >$(CMD_BIN)<)
+     $(error Unable to locate command >$(CMD_BIN)<)
 else
-    ICARUS_BIN_DIR := $(shell dirname $(CMD))
-    export ICARUS_BIN_DIR
+     VCS_BIN_DIR := $(shell dirname $(CMD))
+     export VCS_BIN_DIR
 endif
 
-ifdef TOPLEVEL
-  TOPMODULE_ARG := -s $(TOPLEVEL)
-else
-  TOPMODULE_ARG :=
+ifdef VERILOG_INCLUDE_DIRS
+    COMPILE_ARGS += $(addprefix +incdir+, $(VERILOG_INCLUDE_DIRS))
 endif
 
-COMPILE_ARGS += -f $(SIM_BUILD)/cmds.f -g2012 # Default to latest SystemVerilog standard
+ifeq ($(PYTHON_ARCH),64bit)
+    EXTRA_ARGS += -full64
+endif
 
-# Compilation phase
-$(SIM_BUILD)/sim.vvp: $(VERILOG_SOURCES) $(CUSTOM_COMPILE_DEPS) | $(SIM_BUILD)
-	@echo "+timescale+$(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION)" > $(SIM_BUILD)/cmds.f
-	$(CMD) -o $(SIM_BUILD)/sim.vvp -D COCOTB_SIM=1 $(TOPMODULE_ARG) $(COMPILE_ARGS) $(EXTRA_ARGS) $(VERILOG_SOURCES)
+ifeq ($(GUI),1)
+    EXTRA_ARGS += -gui
+endif
 
-# Execution phase
+# TODO:
+# investigate +vpi+1 option which reduces memory requirements
 
-$(COCOTB_RESULTS_FILE): $(SIM_BUILD)/sim.vvp $(CUSTOM_SIM_DEPS)
-	$(RM) $(COCOTB_RESULTS_FILE)
+# Can't do this using an argument, we have to create a PLI table file
+# enabling write access to the design
+$(SIM_BUILD)/pli.tab : | $(SIM_BUILD)
+	echo "acc+=rw,wn:*" > $@
 
-	MODULE=$(MODULE) TESTCASE=$(TESTCASE) TOPLEVEL=$(TOPLEVEL) TOPLEVEL_LANG=$(TOPLEVEL_LANG) \
-        $(SIM_CMD_PREFIX) $(ICARUS_BIN_DIR)/vvp -M $(shell cocotb-config --lib-dir) -m $(shell cocotb-config --lib-name vpi icarus) $(SIM_ARGS) $(EXTRA_ARGS) $(SIM_BUILD)/sim.vvp $(PLUSARGS)
-
-	$(call check_for_results_file)
+# Compilation phase
+$(SIM_BUILD)/simv: $(VERILOG_SOURCES) $(SIM_BUILD)/pli.tab $(CUSTOM_COMPILE_DEPS) | $(SIM_BUILD)
+	cd $(SIM_BUILD) && \
+	TOPLEVEL=$(TOPLEVEL) \
+	$(CMD) -top $(TOPLEVEL) $(PLUSARGS) +acc+1 +vpi -P pli.tab +define+COCOTB_SIM=1 -sverilog \
+	-timescale=$(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION) \
+	$(EXTRA_ARGS) -debug -load $(shell cocotb-config --lib-name-path vpi vcs) $(COMPILE_ARGS) $(VERILOG_SOURCES)
 
-debug: $(SIM_BUILD)/sim.vvp $(CUSTOM_SIM_DEPS)
-	$(RM) -r $(COCOTB_RESULTS_FILE)
+# Execution phase
+$(COCOTB_RESULTS_FILE): $(SIM_BUILD)/simv $(CUSTOM_SIM_DEPS)
+	$(RM) $(COCOTB_RESULTS_FILE)
 
 	MODULE=$(MODULE) TESTCASE=$(TESTCASE) TOPLEVEL=$(TOPLEVEL) TOPLEVEL_LANG=$(TOPLEVEL_LANG) \
-        $(SIM_CMD_PREFIX) gdb --args $(ICARUS_BIN_DIR)/vvp $(shell cocotb-config --lib-dir) -m $(shell cocotb-config --lib-name vpi icarus) $(SIM_BUILD)/sim.vvp $(SIM_ARGS) $(EXTRA_ARGS) $(PLUSARGS)
+	$(SIM_CMD_PREFIX) $(SIM_BUILD)/simv +define+COCOTB_SIM=1 $(SIM_ARGS) $(EXTRA_ARGS) $(PLUSARGS)
 
 	$(call check_for_results_file)
 
 clean::
 	$(RM) -r $(SIM_BUILD)
+	$(RM) -r simv.daidir
+	$(RM) -r cm.log
+	$(RM) -r ucli.key
 endif
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.ius` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ius`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 ifeq (, $(CMD))
     $(error Unable to locate command >$(CMD_BIN)<)
 else
     IUS_BIN_DIR := $(shell dirname $(CMD))
     export IUS_BIN_DIR
 endif
 
+ifdef VERILOG_INCLUDE_DIRS
+    COMPILE_ARGS += $(addprefix +incdir+, $(VERILOG_INCLUDE_DIRS))
+endif
+
 EXTRA_ARGS += $(COMPILE_ARGS)
 EXTRA_ARGS += $(SIM_ARGS)
 EXTRA_ARGS += -licqueue
 
 ifeq ($(PYTHON_ARCH),64bit)
     EXTRA_ARGS += -64
 endif
@@ -93,21 +97,28 @@
 ifneq ($(VERILOG_SOURCES),)
     HDL_SOURCES += $(VERILOG_SOURCES)
 endif
 else
    $(error A valid value (verilog or vhdl) was not provided for TOPLEVEL_LANG=$(TOPLEVEL_LANG))
 endif
 
+# Builds a list of arguments to support VHDL libraries specified in VHDL_SOURCES_*:
+LIBS := $(foreach LIB, $(VHDL_LIB_ORDER),-makelib $(LIB) $(VHDL_SOURCES_$(LIB)) -endlib)
+
 $(COCOTB_RESULTS_FILE): $(HDL_SOURCES) $(CUSTOM_COMPILE_DEPS) $(CUSTOM_SIM_DEPS) | $(SIM_BUILD)
 	$(RM) $(COCOTB_RESULTS_FILE)
 
+	# Make sure all libs in SOURCES_VHDL_* are mentioned in VHDL_LIB_ORDER and vice versa
+	$(foreach LIB, $(VHDL_LIB_ORDER), $(check_vhdl_sources))
+	$(foreach SOURCES_VAR, $(filter VHDL_SOURCES_%, $(.VARIABLES)), $(check_lib_order))
+
 	set -o pipefail; \
 	MODULE=$(MODULE) TESTCASE=$(TESTCASE) TOPLEVEL=$(TOPLEVEL) GPI_EXTRA=$(GPI_EXTRA) TOPLEVEL_LANG=$(TOPLEVEL_LANG) \
 	$(SIM_CMD_PREFIX) $(CMD) -timescale $(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION) \
-	$(EXTRA_ARGS) $(GPI_ARGS) +access+rwc $(MAKE_LIB) $(HDL_SOURCES) $(PLUSARGS) 2>&1 | tee $(SIM_BUILD)/sim.log
+	$(EXTRA_ARGS) $(GPI_ARGS) +access+rwc $(LIBS) $(MAKE_LIB) $(HDL_SOURCES) $(PLUSARGS) 2>&1 | tee $(SIM_BUILD)/sim.log
 
 	$(call check_for_results_file)
 
 clean::
 	$(RM) -r $(SIM_BUILD)
 	$(RM) -r irun.*
 	$(RM) -r ncsim.*
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.modelsim` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.modelsim`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.questa` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.questa`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ifndef VLOG_ARGS
     VLOG_ARGS = -timescale $(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION) -mfcu
 endif
 
 COMPILE_ARGS += +acc
 
 ifdef VERILOG_INCLUDE_DIRS
-    VLOG_ARGS += +incdir+$(VERILOG_INCLUDE_DIRS)
+    VLOG_ARGS += $(addprefix +incdir+, $(VERILOG_INCLUDE_DIRS))
 endif
 
 # below allows for maintaining legacy syntax as well as enables using cross-simulator vars COMPILE_ARGS/SIM_ARGS
 VLOG_ARGS += $(COMPILE_ARGS)
 VCOM_ARGS += $(COMPILE_ARGS)
 VSIM_ARGS += $(SIM_ARGS)
 
@@ -84,14 +84,15 @@
 VHDL_GPI_INTERFACE ?= fli
 
 ifeq ($(filter vhpi fli,$(VHDL_GPI_INTERFACE)),)
     $(error A valid value (fli or vhpi) was not provided for VHDL_GPI_INTERFACE=$(VHDL_GPI_INTERFACE))
 endif
 
 ifeq ($(TOPLEVEL_LANG),vhdl)
+    VSIM_ARGS += -t $(COCOTB_HDL_TIMEPRECISION)
 ifeq ($(VHDL_GPI_INTERFACE),fli)
     CUSTOM_COMPILE_DEPS += $(FLI_LIB)
     VSIM_ARGS += -foreign \"cocotb_init $(FLI_LIB)\"
 else
     VSIM_ARGS += -voptargs="-access=rw+/." -foreign \"vhpi_startup_routines_bootstrap $(call to_tcl_path,$(VHPI_LIB))\"
 endif
 ifneq ($(VERILOG_SOURCES),)
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.riviera` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.riviera`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,18 @@
 
 ifeq ($(GUI),1)
     CMD += -nosplash
 endif
 
 ALOG_ARGS += -timescale $(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION)
 
+ifdef VERILOG_INCLUDE_DIRS
+    ALOG_ARGS += $(addprefix +incdir+, $(VERILOG_INCLUDE_DIRS))
+endif
+
 # below allows for maintaining legacy syntax as well as enables using cross-simulator vars COMPILE_ARGS/SIM_ARGS
 ALOG_ARGS += $(COMPILE_ARGS)
 ACOM_ARGS += $(COMPILE_ARGS)
 ASIM_ARGS += $(SIM_ARGS)
 
 # Plusargs need to be passed to ASIM command not vsimsa
 ASIM_ARGS += $(PLUSARGS)
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.vcs` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.icarus`

 * *Files 26% similar despite different names*

```diff
@@ -23,72 +23,89 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ###############################################################################
 
+TOPLEVEL_LANG ?= verilog
+
 include $(shell cocotb-config --makefiles)/Makefile.inc
 
-ifneq ($(VHDL_SOURCES),)
+ifneq ($(or $(filter-out $(TOPLEVEL_LANG),verilog),$(VHDL_SOURCES)),)
 
 $(COCOTB_RESULTS_FILE):
-	@echo "Skipping simulation as VHDL is not supported on simulator=$(SIM)"
+	@echo "Skipping simulation as only Verilog is supported on simulator=$(SIM)"
+debug: $(COCOTB_RESULTS_FILE)
 clean::
 
 else
 
-CMD_BIN := vcs
+CMD_BIN := iverilog
 
-ifdef VCS_BIN_DIR
-     CMD := $(shell :; command -v $(VCS_BIN_DIR)/$(CMD_BIN) 2>/dev/null)
+ifdef ICARUS_BIN_DIR
+    CMD := $(shell :; command -v $(ICARUS_BIN_DIR)/$(CMD_BIN) 2>/dev/null)
 else
-     # auto-detect bin dir from system path
-     CMD := $(shell :; command -v $(CMD_BIN) 2>/dev/null)
+    # auto-detect bin dir from system path
+    CMD := $(shell :; command -v $(CMD_BIN) 2>/dev/null)
 endif
 
 ifeq (, $(CMD))
-     $(error Unable to locate command >$(CMD_BIN)<)
+    $(error Unable to locate command >$(CMD_BIN)<)
 else
-     VCS_BIN_DIR := $(shell dirname $(CMD))
-     export VCS_BIN_DIR
+    ICARUS_BIN_DIR := $(shell dirname $(CMD))
+    export ICARUS_BIN_DIR
 endif
 
-ifeq ($(PYTHON_ARCH),64bit)
-    EXTRA_ARGS += -full64
+ifdef TOPLEVEL
+  TOPMODULE_ARG := -s $(TOPLEVEL)
+else
+  TOPMODULE_ARG :=
 endif
 
-ifeq ($(GUI),1)
-    EXTRA_ARGS += -gui
+COMPILE_ARGS += -f $(SIM_BUILD)/cmds.f -g2012 # Default to latest SystemVerilog standard
+
+ifdef VERILOG_INCLUDE_DIRS
+    COMPILE_ARGS += $(addprefix -I, $(VERILOG_INCLUDE_DIRS))
 endif
 
-# TODO:
-# investigate +vpi+1 option which reduces memory requirements
+# Compilation phase
 
-# Can't do this using an argument, we have to create a PLI table file
-# enabling write access to the design
-$(SIM_BUILD)/pli.tab : | $(SIM_BUILD)
-	echo "acc+=rw,wn:*" > $@
+ifeq ($(WAVES), 1)
+    VERILOG_SOURCES += $(SIM_BUILD)/cocotb_iverilog_dump.v
+    COMPILE_ARGS += -s cocotb_iverilog_dump
+    PLUSARGS += -fst
+endif
 
-# Compilation phase
-$(SIM_BUILD)/simv: $(VERILOG_SOURCES) $(SIM_BUILD)/pli.tab $(CUSTOM_COMPILE_DEPS) | $(SIM_BUILD)
-	cd $(SIM_BUILD) && \
-	TOPLEVEL=$(TOPLEVEL) \
-	$(CMD) -top $(TOPLEVEL) $(PLUSARGS) +acc+1 +vpi -P pli.tab +define+COCOTB_SIM=1 -sverilog \
-	-timescale=$(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION) \
-	$(EXTRA_ARGS) -debug -load $(shell cocotb-config --lib-name-path vpi vcs) $(COMPILE_ARGS) $(VERILOG_SOURCES)
+$(SIM_BUILD)/sim.vvp: $(VERILOG_SOURCES) $(CUSTOM_COMPILE_DEPS) | $(SIM_BUILD)
+	@echo "+timescale+$(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION)" > $(SIM_BUILD)/cmds.f
+	$(CMD) -o $(SIM_BUILD)/sim.vvp -D COCOTB_SIM=1 $(TOPMODULE_ARG) $(COMPILE_ARGS) $(EXTRA_ARGS) $(VERILOG_SOURCES)
+
+$(SIM_BUILD)/cocotb_iverilog_dump.v: | $(SIM_BUILD)
+	@echo 'module cocotb_iverilog_dump();' > $@
+	@echo 'initial begin' >> $@
+	@echo '    $$dumpfile("$(SIM_BUILD)/$(TOPLEVEL).fst");' >> $@
+	@echo '    $$dumpvars(0, $(TOPLEVEL));' >> $@
+	@echo 'end' >> $@
+	@echo 'endmodule' >> $@
 
 # Execution phase
-$(COCOTB_RESULTS_FILE): $(SIM_BUILD)/simv $(CUSTOM_SIM_DEPS)
+
+$(COCOTB_RESULTS_FILE): $(SIM_BUILD)/sim.vvp $(CUSTOM_SIM_DEPS)
 	$(RM) $(COCOTB_RESULTS_FILE)
 
 	MODULE=$(MODULE) TESTCASE=$(TESTCASE) TOPLEVEL=$(TOPLEVEL) TOPLEVEL_LANG=$(TOPLEVEL_LANG) \
-	$(SIM_CMD_PREFIX) $(SIM_BUILD)/simv +define+COCOTB_SIM=1 $(SIM_ARGS) $(EXTRA_ARGS) $(PLUSARGS)
+        $(SIM_CMD_PREFIX) $(ICARUS_BIN_DIR)/vvp -M $(shell cocotb-config --lib-dir) -m $(shell cocotb-config --lib-name vpi icarus) $(SIM_ARGS) $(EXTRA_ARGS) $(SIM_BUILD)/sim.vvp $(PLUSARGS)
+
+	$(call check_for_results_file)
+
+debug: $(SIM_BUILD)/sim.vvp $(CUSTOM_SIM_DEPS)
+	$(RM) -r $(COCOTB_RESULTS_FILE)
+
+	MODULE=$(MODULE) TESTCASE=$(TESTCASE) TOPLEVEL=$(TOPLEVEL) TOPLEVEL_LANG=$(TOPLEVEL_LANG) \
+        $(SIM_CMD_PREFIX) gdb --args $(ICARUS_BIN_DIR)/vvp $(shell cocotb-config --lib-dir) -m $(shell cocotb-config --lib-name vpi icarus) $(SIM_BUILD)/sim.vvp $(SIM_ARGS) $(EXTRA_ARGS) $(PLUSARGS)
 
 	$(call check_for_results_file)
 
 clean::
 	$(RM) -r $(SIM_BUILD)
-	$(RM) -r simv.daidir
-	$(RM) -r cm.log
-	$(RM) -r ucli.key
 endif
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.verilator` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.verilator`

 * *Files 23% similar despite different names*

```diff
@@ -32,27 +32,31 @@
 ifdef TOPLEVEL
   TOPMODULE_ARG := --top-module $(TOPLEVEL)
 else
   TOPMODULE_ARG :=
 endif
 
 ifeq ($(VERILATOR_SIM_DEBUG), 1)
-  COMPILE_ARGS += --debug -CFLAGS "-DVL_DEBUG -g"
+  COMPILE_ARGS += --debug -CFLAGS "-DVL_DEBUG -DVERILATOR_SIM_DEBUG -g"
   PLUSARGS += +verilator+debug
   BUILD_ARGS += OPT_FAST=-Og OPT_SLOW=-Og OPT_GLOBAL=-Og
 endif
 
 ifeq ($(VERILATOR_TRACE),1)
   EXTRA_ARGS += --trace --trace-structs
 endif
 
 EXTRA_ARGS += --timescale $(COCOTB_HDL_TIMEUNIT)/$(COCOTB_HDL_TIMEPRECISION)
 
 COMPILE_ARGS += --vpi --public-flat-rw --prefix Vtop -o Vtop -LDFLAGS "-Wl,-rpath,$(shell cocotb-config --lib-dir) -L$(shell cocotb-config --lib-dir) -lcocotbvpi_verilator"
 
+ifdef VERILOG_INCLUDE_DIRS
+  COMPILE_ARGS += $(addprefix +incdir+, $(VERILOG_INCLUDE_DIRS))
+endif
+
 $(SIM_BUILD)/Vtop.mk: $(VERILOG_SOURCES) $(CUSTOM_COMPILE_DEPS) $(COCOTB_SHARE_DIR)/lib/verilator/verilator.cpp | $(SIM_BUILD)
 	$(CMD) -cc --exe -Mdir $(SIM_BUILD) -DCOCOTB_SIM=1 $(TOPMODULE_ARG) $(COMPILE_ARGS) $(EXTRA_ARGS) $(VERILOG_SOURCES) $(COCOTB_SHARE_DIR)/lib/verilator/verilator.cpp
 
 # Compilation phase
 $(SIM_BUILD)/Vtop: $(SIM_BUILD)/Vtop.mk
 	$(MAKE) -C $(SIM_BUILD) $(BUILD_ARGS) -f Vtop.mk
```

### Comparing `cocotb-1.7.2/cocotb/share/makefiles/simulators/Makefile.xcelium` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.xcelium`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 ifeq (, $(CMD))
     $(error Unable to locate command >$(CMD_BIN)<)
 else
     XCELIUM_BIN_DIR := $(shell dirname $(CMD))
     export XCELIUM_BIN_DIR
 endif
 
+ifdef VERILOG_INCLUDE_DIRS
+    COMPILE_ARGS += $(addprefix +incdir+, $(VERILOG_INCLUDE_DIRS))
+endif
+
 EXTRA_ARGS += $(COMPILE_ARGS)
 EXTRA_ARGS += $(SIM_ARGS)
 EXTRA_ARGS += -licqueue
 
 ifeq ($(PYTHON_ARCH),64bit)
     EXTRA_ARGS += -64
 endif
@@ -69,15 +73,15 @@
 ifeq ($(GUI),1)
     EXTRA_ARGS += -gui
 else
     EXTRA_ARGS +=
 endif
 
 # Xcelium errors out if multiple timescales are specified on the command line.
-ifneq (,$(findstring timescale,$(EXTRA_ARGS)))
+ifneq (,$(filter -timescale%,$(EXTRA_ARGS)))
     $(error Please use COCOTB_HDL_TIMEUNIT and COCOTB_HDL_TIMEPRECISION to specify timescale.)
 endif
 
 # Loading the VHPI library causes an error, so we always load the VPI library and supply
 # GPI_EXTRA=$(shell cocotb-config --lib-name-path vhpi xcelium) if needed.
 
 # Xcelium will use default vlog_startup_routines symbol only if VPI library name is libvpi.so
```

### Comparing `cocotb-1.7.2/cocotb/triggers.py` & `cocotb-1.8.0rc1/cocotb/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,30 @@
 
 import abc
 import inspect
 import warnings
 from collections.abc import Awaitable
 from decimal import Decimal
 from numbers import Real
-from typing import Optional, Union
+from typing import Any, Coroutine, Optional, TypeVar, Union
 
 import cocotb
 from cocotb import outcomes, simulator
 from cocotb.log import SimLog
+from cocotb.task import Task
 from cocotb.utils import (
     ParametrizedSingleton,
     get_sim_steps,
     get_time_from_sim_steps,
     lazy_property,
     remove_traceback_frames,
 )
 
+T = TypeVar("T")
+
 
 def _pointer_str(obj):
     """
     Get the memory address of *obj* as used in :meth:`object.__repr__`.
 
     This is equivalent to ``sprintf("%p", id(obj))``, but python does not
     support ``%p``.
@@ -185,14 +188,18 @@
                   Previously this argument was misleadingly called `time_ps`.
 
            units: One of
                ``'step'``, ``'fs'``, ``'ps'``, ``'ns'``, ``'us'``, ``'ms'``, ``'sec'``.
                When *units* is ``'step'``,
                the timestep is determined by the simulator (see :make:var:`COCOTB_HDL_TIMEPRECISION`).
 
+            round_mode (str, optional):
+                String specifying how to handle time values that sit between time steps
+                (one of ``'error'``, ``'round'``, ``'ceil'``, ``'floor'``).
+
         Examples:
 
             >>> await Timer(100, units='ps')
 
             The time can also be a ``float``:
 
             >>> await Timer(100e-9, units='sec')
@@ -774,31 +781,30 @@
     __slots__ = ("triggers",)
 
     def __init__(self, *triggers):
         self.triggers = triggers
 
         # Do some basic type-checking up front, rather than waiting until we
         # await them.
-        allowed_types = (Trigger, Waitable, cocotb.decorators.Task)
+        allowed_types = (Trigger, Waitable, Task)
         for trigger in self.triggers:
             if not isinstance(trigger, allowed_types):
                 raise TypeError(
                     "All triggers must be instances of Trigger! Got: {}".format(
                         type(trigger).__qualname__
                     )
                 )
 
     def __repr__(self):
         # no _pointer_str here, since this is not a trigger, so identity
         # doesn't matter.
         return "{}({})".format(
             type(self).__qualname__,
             ", ".join(
-                repr(Join(t)) if isinstance(t, cocotb.decorators.Task) else repr(t)
-                for t in self.triggers
+                repr(Join(t)) if isinstance(t, Task) else repr(t) for t in self.triggers
             ),
         )
 
 
 async def _wait_callback(trigger, callback):
     """
     Wait for a trigger, and call `callback` with the outcome of the await.
@@ -930,15 +936,20 @@
         if self._type is RisingEdge:
             fmt = "{}({!r}, {!r})"
         else:
             fmt = "{}({!r}, {!r}, rising=False)"
         return fmt.format(type(self).__qualname__, self.signal, self.num_cycles)
 
 
-async def with_timeout(trigger, timeout_time, timeout_unit="step"):
+async def with_timeout(
+    trigger: Union[Trigger, Waitable, Task, Coroutine[Any, Any, T]],
+    timeout_time: Union[float, Decimal],
+    timeout_unit: str = "step",
+    round_mode: Optional[str] = None,
+) -> T:
     r"""
     Waits on triggers or coroutines, throws an exception if it waits longer than the given time.
 
     When a :term:`python:coroutine` is passed,
     the callee coroutine is started,
     the caller blocks until the callee completes,
     and the callee's result is returned to the caller.
@@ -968,20 +979,23 @@
 
     .. code-block:: python
 
         await with_timeout(coro, 100, 'ns')
         await with_timeout(First(coro, event.wait()), 100, 'ns')
 
     Args:
-        trigger (:class:`~cocotb.triggers.Trigger`, :class:`~cocotb.triggers.Waitable`, :class:`~cocotb.decorators.Task`, or :term:`python:coroutine`):
+        trigger (:class:`~cocotb.triggers.Trigger`, :class:`~cocotb.triggers.Waitable`, :class:`~cocotb.task.Task`, or :term:`python:coroutine`):
             A single object that could be right of an :keyword:`await` expression in cocotb.
         timeout_time (numbers.Real or decimal.Decimal):
             Simulation time duration before timeout occurs.
         timeout_unit (str, optional):
             Units of timeout_time, accepts any units that :class:`~cocotb.triggers.Timer` does.
+        round_mode (str, optional):
+            String specifying how to handle time values that sit between time steps
+            (one of ``'error'``, ``'round'``, ``'ceil'``, ``'floor'``).
 
     Returns:
         First trigger that completed if timeout did not occur.
 
     Raises:
         :exc:`SimTimeoutError`: If timeout occurs.
 
@@ -1001,15 +1015,17 @@
         )
         timeout_unit = "step"  # don't propagate deprecated value
     if inspect.iscoroutine(trigger):
         trigger = cocotb.start_soon(trigger)
         shielded = False
     else:
         shielded = True
-    timeout_timer = cocotb.triggers.Timer(timeout_time, timeout_unit)
+    timeout_timer = cocotb.triggers.Timer(
+        timeout_time, timeout_unit, round_mode=round_mode
+    )
     res = await First(timeout_timer, trigger)
     if res is timeout_timer:
         if not shielded:
             trigger.kill()
         raise cocotb.result.SimTimeoutError
     else:
         return res
```

### Comparing `cocotb-1.7.2/cocotb/types/__init__.py` & `cocotb-1.8.0rc1/cocotb/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/types/array.py` & `cocotb-1.8.0rc1/cocotb/types/array.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/types/logic.py` & `cocotb-1.8.0rc1/cocotb/types/logic.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/types/logic_array.py` & `cocotb-1.8.0rc1/cocotb/types/logic_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,29 +24,34 @@
     or from integers.
     If constructed from a positive integer, an unsigned bit representation is used to
     construct the :class:`LogicArray`.
     If constructed from a negative integer, a two's complement bit representation is
     used.
     Like :class:`Array`, if no *range* argument is given, it is deduced from the length
     of the iterable or bit string used to initialize the variable.
+    If a *range* argument is given, but no value,
+    the array is filled with the default value of Logic().
 
     .. code-block:: python3
 
         >>> LogicArray("01XZ")
         LogicArray('01XZ', Range(3, 'downto', 0))
 
         >>> LogicArray([0, True, "X"])
         LogicArray('01X', Range(2, 'downto', 0))
 
-        >>> LogicArray(0xA)                     # picks smallest range that can fit the value
+        >>> LogicArray(0xA)  # picks smallest range that can fit the value
         LogicArray('1010', Range(3, 'downto', 0))
 
-        >>> LogicArray(-4, Range(0, "to", 3))   # will sign-extend
+        >>> LogicArray(-4, Range(0, "to", 3))  # will sign-extend
         LogicArray('1100', Range(0, 'to', 3))
 
+        >>> LogicArray(range=Range(0, "to", 3))  # default values
+        LogicArray('XXXX', Range(0, 'to', 3))
+
     :class:`LogicArray`\ s support the same operations as :class:`Array`;
     however, it enforces the condition that all elements must be a :class:`Logic`.
 
     .. code-block:: python3
 
         >>> la = LogicArray("1010")
         >>> la[0]                               # is indexable
@@ -111,20 +116,46 @@
     Raises:
         ValueError: When argument values cannot be used to construct an array.
         TypeError: When invalid argument types are used.
     """
 
     __slots__ = ()
 
+    @typing.overload
     def __init__(
         self,
         value: typing.Union[int, typing.Iterable[LogicConstructibleT], BinaryValue],
+        range: typing.Optional[Range],
+    ):
+        ...
+
+    @typing.overload
+    def __init__(
+        self,
+        value: typing.Union[
+            int, typing.Iterable[LogicConstructibleT], BinaryValue, None
+        ],
+        range: Range,
+    ):
+        ...
+
+    def __init__(
+        self,
+        value: typing.Union[
+            int, typing.Iterable[LogicConstructibleT], BinaryValue, None
+        ] = None,
         range: typing.Optional[Range] = None,
     ) -> None:
-        if isinstance(value, int):
+        if value is None and range is None:
+            raise ValueError(
+                "at least one of the value and range input parameters must be given"
+            )
+        if value is None:
+            self._value = [Logic() for _ in range]
+        elif isinstance(value, int):
             if value < 0:
                 bitlen = int.bit_length(value + 1) + 1
             else:
                 bitlen = max(1, int.bit_length(value))
             if range is None:
                 self._value = [Logic(v) for v in _int_to_bitstr(value, bitlen)]
             else:
```

### Comparing `cocotb-1.7.2/cocotb/types/range.py` & `cocotb-1.8.0rc1/cocotb/types/range.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/utils.py` & `cocotb-1.8.0rc1/cocotb/utils.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/wavedrom.py` & `cocotb-1.8.0rc1/cocotb/wavedrom.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb/xunit_reporter.py` & `cocotb-1.8.0rc1/cocotb/xunit_reporter.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb.egg-info/PKG-INFO` & `cocotb-1.8.0rc1/cocotb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotb
-Version: 1.7.2
+Version: 1.8.0rc1
 Summary: cocotb is a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 Home-page: https://www.cocotb.org
 Author: Chris Higgs, Stuart Hodgson
 Maintainer: cocotb contributors
 Maintainer-email: cocotb@lists.librecores.org
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cocotb/cocotb/issues
@@ -33,16 +33,15 @@
 [![PyPI](https://img.shields.io/pypi/dm/cocotb.svg?label=PyPI%20downloads)](https://pypi.org/project/cocotb/)
 [![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/cocotb/cocotb)
 [![codecov](https://codecov.io/gh/cocotb/cocotb/branch/master/graph/badge.svg)](https://codecov.io/gh/cocotb/cocotb)
 
 * Read the [documentation](https://docs.cocotb.org)
 * Get involved:
   * [Raise a bug / request an enhancement](https://github.com/cocotb/cocotb/issues/new) (Requires a GitHub account)
-  * [Join the mailing list](https://lists.librecores.org/listinfo/cocotb)
-  * [Join the Gitter chat room](https://gitter.im/cocotb)
+  * [Join the Gitter chat room](https://gitter.im/cocotb/Lobby)
 
 ## Installation
 
 The current stable version of cocotb requires:
 
 - Python 3.6+
 - GNU Make 3+
@@ -92,30 +91,46 @@
 
 An example of a simple randomized cocotb testbench:
 
 ```python
 # test_dff.py
 
 import random
+
 import cocotb
 from cocotb.clock import Clock
-from cocotb.triggers import FallingEdge
+from cocotb.triggers import RisingEdge
+from cocotb.types import LogicArray
 
 @cocotb.test()
-async def test_dff_simple(dut):
-    """ Test that d propagates to q """
+async def dff_simple_test(dut):
+    """Test that d propagates to q"""
+
+    # Assert initial output is unknown
+    assert LogicArray(dut.q.value) == LogicArray("X")
+    # Set initial input value to prevent it from floating
+    dut.d.value = 0
 
     clock = Clock(dut.clk, 10, units="us")  # Create a 10us period clock on port clk
-    cocotb.start_soon(clock.start())  # Start the clock
+    # Start the clock. Start it low to avoid issues on the first RisingEdge
+    cocotb.start_soon(clock.start(start_high=False))
 
+    # Synchronize with the clock. This will regisiter the initial `d` value
+    await RisingEdge(dut.clk)
+    expected_val = 0  # Matches initial input value
     for i in range(10):
         val = random.randint(0, 1)
         dut.d.value = val  # Assign the random value val to the input port d
-        await FallingEdge(dut.clk)
-        assert dut.q.value == val, "output q was incorrect on the {}th cycle".format(i)
+        await RisingEdge(dut.clk)
+        assert dut.q.value == expected_val, f"output q was incorrect on the {i}th cycle"
+        expected_val = val # Save random value for next RisingEdge
+
+    # Check the final input on the next clock
+    await RisingEdge(dut.clk)
+    assert dut.q.value == expected_val, "output q was incorrect on the last cycle"
 ```
 
 A simple Makefile:
 
 ```make
 # Makefile
```

### Comparing `cocotb-1.7.2/cocotb.egg-info/SOURCES.txt` & `cocotb-1.8.0rc1/cocotb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 cocotb/memdebug.py
 cocotb/outcomes.py
 cocotb/queue.py
 cocotb/regression.py
 cocotb/result.py
 cocotb/runner.py
 cocotb/scheduler.py
+cocotb/task.py
 cocotb/triggers.py
 cocotb/utils.py
 cocotb/wavedrom.py
 cocotb/xunit_reporter.py
 cocotb.egg-info/PKG-INFO
 cocotb.egg-info/SOURCES.txt
 cocotb.egg-info/dependency_links.txt
```

### Comparing `cocotb-1.7.2/cocotb.egg-info/top_level.txt` & `cocotb-1.8.0rc1/cocotb.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/cocotb_build_libs.py` & `cocotb-1.8.0rc1/cocotb_build_libs.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/pygpi/entry.py` & `cocotb-1.8.0rc1/pygpi/entry.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/pyproject.toml` & `cocotb-1.8.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cocotb-1.7.2/setup.cfg` & `cocotb-1.8.0rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,28 @@
 	W503  # line break before binary operator (black)
 per-file-ignores = 
 	examples/doc_examples/quickstart/test_my_design.py: E402,F811
 
 [tool:pytest]
 testpaths = 
 	tests/pytest
-	examples/simple_dff
 markers = 
 	simulator_required: mark tests as needing a simulator
+	compile: the compile step in runner-based tests
 
 [coverage:run]
 omit = 
 	*/cocotb/config.py
 	*/cocotb/_vendor/*
 
+[coverage:paths]
+source = 
+	cocotb/
+	.nox/**/cocotb/
+
 [coverage:report]
 omit = 
 	*/cocotb/config.py
 	*/cocotb/_vendor/*
 exclude_lines = 
 	pragma: no cover
 	\.\.\.
```

### Comparing `cocotb-1.7.2/setup.py` & `cocotb-1.8.0rc1/setup.py`

 * *Files identical despite different names*

