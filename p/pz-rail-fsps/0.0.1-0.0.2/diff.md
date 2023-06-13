# Comparing `tmp/pz-rail-fsps-0.0.1.tar.gz` & `tmp/pz-rail-fsps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-fsps-0.0.1.tar", last modified: Thu Sep 15 15:33:27 2022, max compression
+gzip compressed data, was "pz-rail-fsps-0.0.2.tar", last modified: Tue Jun 13 20:31:39 2023, max compression
```

## Comparing `pz-rail-fsps-0.0.1.tar` & `pz-rail-fsps-0.0.2.tar`

### file list

```diff
@@ -1,85 +1,36 @@
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.478504 pz-rail-fsps-0.0.1/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      123 2022-09-15 00:24:59.000000 pz-rail-fsps-0.0.1/.flake8
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.436550 pz-rail-fsps-0.0.1/.github/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.439068 pz-rail-fsps-0.0.1/.github/workflows/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     2218 2022-09-15 02:41:34.000000 pz-rail-fsps-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      548 2022-09-15 00:25:56.000000 pz-rail-fsps-0.0.1/.github/workflows/pypi.yaml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1811 2022-09-15 02:20:02.000000 pz-rail-fsps-0.0.1/.gitignore
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1102 2022-09-15 00:24:43.000000 pz-rail-fsps-0.0.1/LICENSE
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1924 2022-09-15 15:33:27.478290 pz-rail-fsps-0.0.1/PKG-INFO
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       35 2022-09-15 00:24:43.000000 pz-rail-fsps-0.0.1/README.md
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3089 2022-09-15 15:29:11.000000 pz-rail-fsps-0.0.1/pyproject.toml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       38 2022-09-15 15:33:27.478566 pz-rail-fsps-0.0.1/setup.cfg
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       71 2022-09-15 15:30:11.000000 pz-rail-fsps-0.0.1/setup.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.436838 pz-rail-fsps-0.0.1/src/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.439986 pz-rail-fsps-0.0.1/src/pz_rail_fsps.egg-info/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1924 2022-09-15 15:33:27.000000 pz-rail-fsps-0.0.1/src/pz_rail_fsps.egg-info/PKG-INFO
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3631 2022-09-15 15:33:27.000000 pz-rail-fsps-0.0.1/src/pz_rail_fsps.egg-info/SOURCES.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)        1 2022-09-15 15:33:27.000000 pz-rail-fsps-0.0.1/src/pz_rail_fsps.egg-info/dependency_links.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       63 2022-09-15 15:33:27.000000 pz-rail-fsps-0.0.1/src/pz_rail_fsps.egg-info/requires.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)        5 2022-09-15 15:33:27.000000 pz-rail-fsps-0.0.1/src/pz_rail_fsps.egg-info/top_level.txt
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.437092 pz-rail-fsps-0.0.1/src/rail/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.436984 pz-rail-fsps-0.0.1/src/rail/creation/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.440825 pz-rail-fsps-0.0.1/src/rail/creation/sed_generation/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       88 2022-09-15 01:49:26.000000 pz-rail-fsps-0.0.1/src/rail/creation/sed_generation/__init__.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      176 2022-09-15 15:33:27.000000 pz-rail-fsps-0.0.1/src/rail/creation/sed_generation/_version.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     2457 2022-09-15 01:33:02.000000 pz-rail-fsps-0.0.1/src/rail/creation/sed_generation/generator.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    11386 2022-09-15 01:33:02.000000 pz-rail-fsps-0.0.1/src/rail/creation/sed_generation/sed_generator.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.437435 pz-rail-fsps-0.0.1/src/rail/examples/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.437244 pz-rail-fsps-0.0.1/src/rail/examples/estimation/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.437327 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.477206 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    26196 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/El_B2004a.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    31348 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/El_B2004a.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    28901 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/El_B2004a.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    23092 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/El_B2004a.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    37073 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/El_B2004a.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    33480 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/El_B2004a.DC2LSST_z.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    26237 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Im_B2004a.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    31529 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Im_B2004a.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    28867 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Im_B2004a.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    23081 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Im_B2004a.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    37001 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Im_B2004a.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    33806 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Im_B2004a.DC2LSST_z.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    26062 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB2_B2004a.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    31621 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB2_B2004a.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    29040 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB2_B2004a.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    23008 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB2_B2004a.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    36953 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB2_B2004a.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    33726 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB2_B2004a.DC2LSST_z.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    26239 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB3_B2004a.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    31518 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB3_B2004a.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    28891 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB3_B2004a.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    23074 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB3_B2004a.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    36986 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB3_B2004a.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    33713 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/SB3_B2004a.DC2LSST_z.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    26198 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Sbc_B2004a.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    31432 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Sbc_B2004a.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    28934 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Sbc_B2004a.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    23066 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Sbc_B2004a.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    36997 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Sbc_B2004a.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    33746 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Sbc_B2004a.DC2LSST_z.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    26295 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Scd_B2004a.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    31594 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Scd_B2004a.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    29155 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Scd_B2004a.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    22882 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Scd_B2004a.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    36717 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Scd_B2004a.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    33624 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/Scd_B2004a.DC2LSST_z.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38677 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_25Myr_z008.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38733 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_25Myr_z008.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38677 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_25Myr_z008.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38584 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_25Myr_z008.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38551 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_25Myr_z008.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38594 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_25Myr_z008.DC2LSST_z.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38553 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_5Myr_z008.DC2LSST_g.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38638 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_5Myr_z008.DC2LSST_i.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38757 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_5Myr_z008.DC2LSST_r.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38514 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_5Myr_z008.DC2LSST_u.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38664 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_5Myr_z008.DC2LSST_y.AB
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    38688 2022-09-15 01:41:58.000000 pz-rail-fsps-0.0.1/src/rail/examples/estimation/data/AB/ssp_5Myr_z008.DC2LSST_z.AB
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.477811 pz-rail-fsps-0.0.1/src/rail/examples/testdata/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       73 2022-09-15 15:29:11.000000 pz-rail-fsps-0.0.1/src/rail/examples/testdata/lsf_bad_wave_array.dat
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       41 2022-09-15 15:29:11.000000 pz-rail-fsps-0.0.1/src/rail/examples/testdata/sfh_bad_age_array.dat
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    11520 2022-09-15 02:04:47.000000 pz-rail-fsps-0.0.1/src/rail/examples/testdata/test_fsps_sed.fits
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2022-09-15 15:33:27.477989 pz-rail-fsps-0.0.1/tests/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     8406 2022-09-15 02:12:07.000000 pz-rail-fsps-0.0.1/tests/test_sed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.008233 pz-rail-fsps-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.008233 pz-rail-fsps-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2250 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.008233 pz-rail-fsps-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/src/pz_rail_fsps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-13 20:31:38.000000 pz-rail-fsps-0.0.2/src/pz_rail_fsps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-06-13 20:31:38.000000 pz-rail-fsps-0.0.2/src/pz_rail_fsps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 20:31:38.000000 pz-rail-fsps-0.0.2/src/pz_rail_fsps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 20:31:38.000000 pz-rail-fsps-0.0.2/src/pz_rail_fsps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 20:31:38.000000 pz-rail-fsps-0.0.2/src/pz_rail_fsps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.008233 pz-rail-fsps-0.0.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/src/rail/added_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    13137 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/src/rail/added_examples/sed_gen_fsps-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.008233 pz-rail-fsps-0.0.2/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/src/rail/creation/sed_generation/
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/src/rail/creation/sed_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 20:31:38.000000 pz-rail-fsps-0.0.2/src/rail/creation/sed_generation/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/src/rail/creation/sed_generation/generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11473 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/src/rail/creation/sed_generation/sed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.008233 pz-rail-fsps-0.0.2/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/src/rail/examples_data/testdata/lsf_bad_wave_array.dat
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/src/rail/examples_data/testdata/sfh_bad_age_array.dat
+-rw-r--r--   0 runner    (1001) docker     (122)    11520 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/src/rail/examples_data/testdata/test_fsps_sed.fits
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:31:39.012234 pz-rail-fsps-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8421 2023-06-13 20:31:25.000000 pz-rail-fsps-0.0.2/tests/test_sed_generator.py
```

### Comparing `pz-rail-fsps-0.0.1/.github/workflows/main.yml` & `pz-rail-fsps-0.0.2/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        pip install wheel numpy
         pip install .
         pip install flake8 pytest pytest-cov mockmpi pytest-timeout
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Install fsps
       run: |
         git clone https://github.com/cconroy20/fsps.git /opt/hostedtoolcache/Python/fsps
     - name: Test with pytest
```

### Comparing `pz-rail-fsps-0.0.1/.github/workflows/pypi.yaml` & `pz-rail-fsps-0.0.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.0.1/.gitignore` & `pz-rail-fsps-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.0.1/LICENSE` & `pz-rail-fsps-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.0.1/PKG-INFO` & `pz-rail-fsps-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-fsps
-Version: 0.0.1
+Version: 0.0.2
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <none@none.gov>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-fsps-0.0.1/pyproject.toml` & `pz-rail-fsps-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,21 @@
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
     "fsps",
-    "pz-rail",
+    "pz-rail-base",
+    "astropy",
 ]
 
 [project.optional-dependencies]
 dev = [
+    "qp-prob[full]",
     "coverage",
     "pylint",
     "pytest",
     "pytest-cov",
     "yamllint",
 ]
```

### Comparing `pz-rail-fsps-0.0.1/src/pz_rail_fsps.egg-info/PKG-INFO` & `pz-rail-fsps-0.0.2/src/pz_rail_fsps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-fsps
-Version: 0.0.1
+Version: 0.0.2
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <none@none.gov>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-fsps-0.0.1/src/rail/creation/sed_generation/generator.py` & `pz-rail-fsps-0.0.2/src/rail/creation/sed_generation/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Abstract base class defining a generator
 
 The key feature is that the __call__ method takes a TableHandle and
-and returns a FitsHandle, and wraps the run method
+returns a FitsHandle, and wraps the run method
 """
 
 from rail.core.stage import RailStage
 from rail.core.data import TableHandle, FitsHandle
 
 
 class SedGenerator(RailStage):
@@ -21,15 +21,16 @@
     inputs = [('input', TableHandle)]
     outputs = [('output', FitsHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Generator that can create rest-frame SEDs"""
         RailStage.__init__(self, args, comm=comm)
 
-    def __call__(self, sample, seed: int = None, physical_units=True, tabulated_sfh_file=None, tabulated_lsf_file=None):
+    def __call__(self, sample, seed: int = None, physical_units=True, tabulated_sfh_file=None, 
+                 tabulated_lsf_file=None): # pragma: no cover
         """The main interface method for `Generator`
 
         Generate SEDs.
 
         This will attach the sample to this `Generator`
         (for introspection and provenance tracking).
```

### Comparing `pz-rail-fsps-0.0.1/src/rail/creation/sed_generation/sed_generator.py` & `pz-rail-fsps-0.0.2/src/rail/creation/sed_generation/sed_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,18 @@
                     'add_neb_emission must be set to False when using tabular SFHs'
                 age_array, sfr_array, metal_array = np.loadtxt(tabulated_sfh_file, usecols=(0, 1, 2))
                 sp.set_tabular_sfh(age_array, sfr_array, Z=metal_array)
 
             if self.config.smooth_lsf:
                 assert self.config.smooth_velocity is True, 'lsf smoothing only works if smooth_velocity is True'
                 lsf_values = np.loadtxt(tabulated_lsf_file, usecols=(0, 1))
-                wave = lsf_values[:, 0]
-                sigma = lsf_values[:, 1]
-                sp.set_lsf(wave, sigma, wmin=self.config.min_wavelength, wmax=self.config.max_wavelength)
+                wave = lsf_values[:, 0]  # pragma: no cover
+                sigma = lsf_values[:, 1]  # pragma: no cover
+                sp.set_lsf(wave, sigma, wmin=self.config.min_wavelength,
+                           wmax=self.config.max_wavelength)  # pragma: no cover
 
             wavelength, flux_solar_lum_angstrom = sp.get_spectrum(tage=ages[i], peraa=True)
 
             selected_wave_range = np.where((wavelength >= self.config.min_wavelength) &
                                            (wavelength <= self.config.max_wavelength))
             wavelength = wavelength[selected_wave_range]
             wavelengths[i] = wavelength
```

### Comparing `pz-rail-fsps-0.0.1/src/rail/examples/testdata/test_fsps_sed.fits` & `pz-rail-fsps-0.0.2/src/rail/examples_data/testdata/test_fsps_sed.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.0.1/tests/test_sed_generator.py` & `pz-rail-fsps-0.0.2/tests/test_sed_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tables_io
 from rail.creation.sed_generation import FSPSSedGenerator
 import pytest
 from rail.core.stage import RailStage
 import numpy as np
 
 from rail.core.utils import RAILDIR
-test_data = os.path.join(RAILDIR, 'rail', 'examples', 'testdata', 'test_fsps_sed.fits')
+test_data = os.path.join(RAILDIR, 'rail', 'examples_data', 'testdata', 'test_fsps_sed.fits')
 
 
 @pytest.mark.parametrize(
     "settings,error",
     [
         ({"min_wavelength": -1}, ValueError),
         ({"max_wavelength": -1}, ValueError),
@@ -93,15 +93,15 @@
 )
 def test_FSPSSedGenerator_wrong_age_tabulated_sfh_file(settings, error):
     """Test bad tabulated sfh params that should raise Value and Type errors."""
     with pytest.raises(error):
         DS = RailStage.data_store
         DS.__class__.allow_overwrite = True
         dummy_io_data = tables_io.read(test_data)
-        sfh_file = os.path.join(RAILDIR, 'rail', 'examples', 'testdata', 'sfh_bad_age_array.dat')
+        sfh_file = os.path.join(RAILDIR, 'rail', 'examples_data', 'testdata', 'sfh_bad_age_array.dat')
         sed_generation_test = FSPSSedGenerator.make_stage(name='sed_generator_test', zcontinuous=3,
                                                           add_neb_emission=False, physical_units=True,
                                                           tabulated_sfh_file=sfh_file,
                                                           tabulated_lsf_file=None,
                                                           **settings)
         sed_generation_test.add_data('input', dummy_io_data)
         sed_generation_test.run()
@@ -153,15 +153,15 @@
 )
 def test_FSPSSedGenerator_wrong_wavelength_tabulated_lsf_file(settings, error):
     """Test bad tabulated sfh params that should raise Value and Type errors."""
     with pytest.raises(error):
         DS = RailStage.data_store
         DS.__class__.allow_overwrite = True
         dummy_io_data = tables_io.read(test_data)
-        lsf_file = os.path.join(RAILDIR, 'rail', 'examples', 'testdata', 'lsf_bad_wave_array.dat')
+        lsf_file = os.path.join(RAILDIR, 'rail', 'examples_data', 'testdata', 'lsf_bad_wave_array.dat')
         sed_generation_test = FSPSSedGenerator.make_stage(name='sed_generator_test', smooth_velocity=True,
                                                           physical_units=True, tabulated_sfh_file=None,
                                                           tabulated_lsf_file=lsf_file,
                                                           **settings)
         sed_generation_test.add_data('input', dummy_io_data)
         sed_generation_test.run()
```

